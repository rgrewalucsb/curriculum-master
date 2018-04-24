# CSS Friends

## Phase 5: Cats

**Topics:** [Background-size][t-background-size],
[Positioning][t-positioning], [Text-shadow][t-text-shadow]

- [Screenshot A][ss-05-a]
- [Screenshot B][ss-05-b]
- [Live][live-05]

Create a `.content-header` section and put it at the top inside of the
`.content` container, above the sidebar and main section. Give it a
height and use the supplied `../docs/images/cats.jpg` image as a
background. Make sure the background image covers the full section.

Add a heading and button and position them absolute at the bottom. To
keep the heading legible on a varied background, use the `text-shadow`
property to increase contrast.

For headings with a large `font-size` that do not wrap multiple lines,
we like to decrease the `line-height` as it will add a decent chunk of
additional space above and below the words, which is only needed if we
have multiple lines. Let's get rid of that space by setting
`line-height` to `1` on our header.

[ss-05-a]: ../docs/screenshots/05-cats-a.png
[ss-05-b]: ../docs/screenshots/05-cats-b.png
[live-05]: http://appacademy.github.io/css-friends/solution/05-cats.html

[t-background-size]: https://developer.mozilla.org/en-US/docs/Web/CSS/background-size
[t-text-shadow]: https://developer.mozilla.org/en-US/docs/Web/CSS/text-shadow
[t-line-height]: http://css-tricks.com/almanac/properties/l/line-height/
[t-positioning]: https://github.com/appacademy/css-demos/#positioning
