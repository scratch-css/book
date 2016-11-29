### Rules

Using Scratch requires to follow some rules to get good result. I give you todoes and not todoes list here. They are also good for performant CSS in general.

#### CSS

- Never hardcode these values and properties:
  - Hex or rgb(a) colors - see [Colors](colors.html).
  - Any unit in any value - see [Units](units.html).
  - Font weight or style - see [Typography](typography.html).
  - Paddings and margins - see [Gutters](gutter.html).
  - Time units, durations and delays - see [Time](time.html).
- Never nest classes more then 3 levels - see [Performance](performance.html).
- Never use universal selector `*` - see [Performance](performance.html).
- Try to avoid attribute selectors and pseudo classes - see [Performance](performance.html).
- Move to variables if you use it more than once - see [Variables](variables.html).
- Check [Scratch quick reference](https://github.com/scratch-css/quick-reference) before you add something new (use `ctrl`/`cmd` + `F` to find them quickly).

#### HTML
- You can have modifier as a separate class name. No need extra characters to use (`button big primary` instead of `button-primary-big` or `contact--button__red`).
- Avoid wrappers, as much as possible. 

