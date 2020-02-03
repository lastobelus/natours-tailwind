# PostCSS plugins to be near-sasslike

`postcss-import` -- import statements, but they _must_ be at the top
`postcss-nested` -- nesting, almost identical to scss
`postcss-custom-properties` -- variables with css properties style syntax. There is `postcss-simple-vars`, which is sass style vars, but they don't have maps anyway, and --var is easier to type then $var
`postcss-functions` -- functions, but you write them in javascript!


## Undecided
`postcss-mixins` -- can write mixins in javascript, but the parameter syntax is `postcss-simple-vars`, and `postcss-simple-vars` is a dependency. So it would mean mixing two variable/parameter syntaxes unless I ditch postcss-custom-properties
`postcss-preset-env` -- a grab bag of mildly useful things. A version of nesting where need a space after the &. variables similar to postcss-custom-properties. Color functions, but they're weird syntax with no commas.
`postcss-color-function` -- based on css spec, color functions with weird syntax. There are some plugins that try to be more sass-like, but they are unmaintained/deprecated and not quite sass anyway. So will probably have to go with and adjust to this. 
`postcss-url` -- rebase urls (so can write `url(images/bob.png)` when the images are actually in (for example) `../../some/folder/image`)
`postcss-easings` -- easings from https://easings.net/en -- awesome, should use
`postcss-scss` -- parse scss mixins as @rules, and scss variables as properties
`postcss-utilities` -- a bunch of useful utilities. Useful if only for triangles
`postcss-write-svg` -- declarative syntax for writing simple svg inline in css

# Alternatives
`precss` -- https://github.com/jonathantneal/precss, uses postcss-advanced-variables, postcss-atroot, postcss-extend-rule, postcss-nested, postcss-preset-env, postcss-property-lookup
gives you $vars, everywhere. But may be out-of-date? last updates 15mo ago