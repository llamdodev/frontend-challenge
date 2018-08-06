# frontend-challenge

The repository includes some data after our processing, and leaves it up to your inspiration
to display it in a nice way. We have attached the way we chose (for now) [in the annex](#annex).

## Submit

Please add @laurentsigal as a contributor to your github repository.

Otherwise you can simply host the code anywhere and give us a link to the zip file.

Do not make your repository public.

## The data

We have attached the file `comparisons.json`.
It corresponds to the comparison of a list of flows between 2 versions of an app. The versions
are denoted by `head` for the latest version, and `base` for the stable version compared against.

Each `head` and `base` have the same structure, that is a collection of keyed steps.
The key allows to map the step from `head `to the corresponding step from `base`.
It might be (case for the label #3 for instance) that a step is included in one version only.

Steps themselves include:
- **interaction**: the user input that was produced during that step to lead to the next one. It has
an interaction type, and optionally a corresponding box on the screen (e.g. where was the element clicked).
- **screenUrl**: the screenshot where that interaction took place
- **diffNodes**: an indexed collection of the nodes that changed between `head` and `base`:
  * the key allows to find (if any) the corresponding node in the other version.
  * the box allows to emphasize the proper area of the screen where that happened.

## Guidelines

- Code in Reactjs
- We should be able to run the code on our end in a few steps
- We tend to pay attention to the organization of code.
- Bonus point if you can tackle label #3 and label #4 (where `head` has more steps than `base`), but
start with simple
- Try to impress us :-)

## Annex

![demo](https://user-images.githubusercontent.com/10992081/41192660-855295a4-6c01-11e8-9095-77b38d928bcf.gif)
