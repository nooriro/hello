# Cross-browser differences with `word-wrap/overflow-wrap: break-word` around float

## Related links

- Static HTML: [overflow-wrap-around-float.html](https://nooriro.github.io/hello/230415-overflow-wrap-around-float/overflow-wrap-around-float.html) \([View in GitHub](overflow-wrap-around-float.html)\)
- CodePen: <https://codepen.io/nooriro/full/QWZNqeQ>
- Stack Overflow:

## Different results in different browsers




Scroll left and right to see all the results.

<table>
  <thead>
    <tr>
      <th>Result in Chrome 112</th>
      <th>Result in Safari 14.1.2</th>
      <th>Result in Firefox 112</th>
    </tr>
  </thead>
  <tbody align="center" valign="top">
    <tr>
      <td><img src="overflow-wrap-around-float-android-chrome-112-230415.png" alt="overflow-wrap-around-float-android-chrome-112-230415" width="368"></td>
      <td><img src="overflow-wrap-around-float-ios-safari-14_1_2-230415.png" alt="overflow-wrap-around-float-ios-safari-14_1_2-230415" width="368"></td>
      <td><img src="overflow-wrap-around-float-android-firefox-112-230415.png" alt="overflow-wrap-around-float-android-firefox-112-230415" width="368"></td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td>&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&ensp;</td>
      <td>&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&ensp;</td>
      <td>&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&ensp;</td>
    </tr>
  </tfoot>
</table>

The results are all different from the others.

- **Chrome:** Both non-link and link text are wrapped around the floated box. This is the result that I expected.
- **Safari:** Only non-link text is wrapped around the floated box.
- **Firefox:** Neither non-link nor link text is wrapped around the floated box.

Tested on Android 10 `QQ3A.200805.001` on Google Pixel 3 XL (Chrome, Firefox) and iOS 14.8 `18H17` on Apple iPhone 6s (Safari).
