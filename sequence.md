## Sequence

Scratch sequences are constants, which represent by what sequences different CSS properties should increase. This is highly inspired by [type-scale.com](http://type-scale.com/). In this website, you can see few constants which directly come from the nature. For example `golden-ratio` is a constant which equals to a mathematical Φ (`phi`), which nearly equals to `1.618`.

Lets say, our sequence for transition duration equals to `var(--golden-ratio)` (which is `1.618`). Lets also say, our default `transition-duration` is `0.3s`.

Now, we can make new unit for our next, bigger duration `transition-duration-big`. To calculate it, we say: `transition-duration-big` equals to `transition-duration` `*` `transition-duration-sequence`, i.e. `--transition-duration-big: var(--transition-duration) * var(--transition-duration-sequence)` => `--transition-duration-big: 0.3s * 1.618` ≈ `0.485`.

Lets make set for our transition durations:
- `transition-duration-shorter: transition-duration-short / golden-ratio` ≈ `0.114s`
- `transition-duration-short: transition-duration / golden-ratio` ≈ `0.185s`
- `transition-duration: 0.3s`
- `transition-duration-long: transition-duration * golden-ratio` ≈ `0.485`
- `transition-duration-longer: transition-duration-long * golden-ratio` ≈ `0.785`

We've got pretty good set right?

The same technique should apply to every CSS property in which we may have more than 1 values.

Referenced from [type-scale.com](http://type-scale.com/), we have those constants:
- `minor-second` -  `1.067`
- `major-second` -  `1.125`
- `minor-third` -  `1.2`
- `major-third` -  `1.25`
- `perfect-fourth` -  `1.333`
- `augmented-fourth` -  `1.414`
- `perfect-fifth` -  `1.5`
- `golden-ratio` -  `1.618`

We can set different sequences for different properties, like `golden-ratio` for `gutters` (see [Gutters](gutters.html)), `major-third` for `headings` (like `h1`, `h2` etc - see [Headings](headings.html)) and so on.