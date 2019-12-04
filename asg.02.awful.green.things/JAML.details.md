# JAML

JAML (or Jordan's Awesome Markup Language) is a file format that I just made up. It's based on YAML (yes, that's a thing), but you probably don't care about that.

In phase 03 of the assignment, we use these files to capture the data about what monsters are in the three areas of The Passageway. You're going to read from and write to these files in JAML format, so let's talk about the format.

Here we go.

## An example

Here's an example of a file (`passageway.mdf`) in YAML format:

```yaml
# area one - a comment is optional
area_start
	- stunned_babies: 2
	- adults: 14
	- stunned_fragments: 6
	- eggs: 10
	- stunned_egg: 12
area_done

area_start
	- babies: 4
area_done

# this is a comment, too
#and another! without a space after the hash mark! Madness!

area_start
	- stunned_adults: 3
area_done
```

We'll refer to this example in the next section.

## The Next Section

For the current application to work, all JAML files need to end with the extension `.mdf`. It stands for "monster data file". How droll.

A JAML file has the following parts:

### comments (optional)

- comments start with a # character
- everything after the # on the same line is ignored
- comments have to be on their own line; unlike a Java "//"
- comments cannot go anywhere between a `area_start`-`area_done` block

### exactly 3 `area_start` - `area_done` sections

- each section starts with exactly the text area_start and has 0 or more lines of `area content`

### `area content` lines

- begin with an optional tab,
- then a mandatory dash,
- then a mandatory space,
- then a `life stage description`,
- then a colon,
- then a space,
- and finally an integer >= 0

### `life stage description` line

- must be one of
  - **adults**
  - **stunned_adults**
  - **babies**
  - **stunned_babies**
  - **fragments**
  - **stunned_fragments**
  - **eggs**
  - **stunned_eggs**
- these lines can be in any order!

## A Confession

My tests for this section are pretty lenient - parsing a text file that has a format like this can be surprisingly challenging and I've done an admittedly slapdash job of building these particular tests. So there's a good chance you might craft a solution to MonsterReader and MonsterWriter that doesn't "really" follow the JAML specs.

Such is life!

## Further Examples

Just in case you find these useful, here are some example mdf files with some commentary:

```yaml
area_start
area_done

area_start
area_done

area_start
area_done
```

_This represents an empty passageway - all 3 areas are empty of Green Things. Thank Odin!_

```yaml
area_start
area_done

area_start
	- adults: 4
	- stunned_adults: 11
	- stunned_babies: 2
	- stunned_fragments: 8
	- eggs: 1
area_done

area_start
	- stunned_adults: 3
	- stunned_eggs: 4
area_done
```

_This file shows a Passageway where the first area is empty, the second area has a crapload of stunned adults and fragments (plus some other Things), and the third area a smattering of stunned adults and eggs._

```yaml
area_start
	- adults: 4
	- stunned_babies: 2
	- stunned_fragments: 99
	- stunned_eggs: 10
area_done

area_start
area_done

area_start
	- stunned_adults: 8
	- babies: 4
area_done
```

_OMG! THAT IS A LOT OF STUNNED FRAGMENTS IN THE FIRST AREA. Good thing the second area is empty._
