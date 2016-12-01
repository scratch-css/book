### Configuring sequence

There are many properties in CSS which can use our sequence system. By default, in Scratch, we have sequences representing:

- Font sizes
- Gutters
- Durations
- And all other properties where we have more than one value.

For example, we want to change headings sequence. If we look [at the code](https://github.com/scratch-css/scratch/blob/master/lib/config/typography/headings.css#L15) in Scratch, `--headings-sequence` is bound to a `--font-sequence`, which is default value for all font related sequences. In its own, it is defined [here](https://github.com/scratch-css/scratch/blob/master/lib/config/typography/font.css#L30). Now, we know that, by default, both `headings-sequence` and `--font-sequence` constants equal to `--major-second`, which is `1.125`. Remember that, if we change `--font-sequence` and don't touch `--headings-sequence`, they will still stay on the same value. But if we change `--headings-sequence`, it will get new value and `--font-sequence` actions will not affect on it anymore.

So, we want new value for headings sequence. Let's choose `--major-third` constant for new one. We can make new CSS file in our project folder, call it `typography/headings.css` and put this snippet:

```
:root {
  --headings-sequence: var(--major-third);
}
```

Now we have new headings sequence value, which will automatically affect all your headings in your HTML, because they are set in the same file, which, in the end are used in our [reset.css](https://github.com/scratch-css/scratch/blob/master/lib/config/typography/headings.css#L19).

This was just an example about how to use sequences in your Scratch project. For more reading about specifically headings, you can see [Headings](headings.html) section.