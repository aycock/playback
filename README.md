# playback
Live coding recording and playback.

How it works:
1. Run the record.sh script in the terminal window whose interactions you want to record. This
  requires a version of `script` that supports the `--timing` option.
2. When you're done recording, exit `script`'s subshell and copy the `.script` and `.tm` files
  to your friendly neighborhood web server; don't forget to make them world-readable.  You'll
  also need to place `index.html` there, along
  with [`pikaday.js`](https://github.com/dbushell/Pikaday) and `pikaday.css`, and
  [`term.js`](https://github.com/chjj/term.js).
3. Edit `index.html` to add the new entry into the meaningfully named `V`.
4. Lather, rinse, repeat.

When you first install `index.html`, you'll need to update `URLBASE` appropriately for your
site, adjust `minDate`, `maxDate`, and `yearRange` for your semester, and replace `CPSC 231`
with your course name.

John Aycock (aycock@ucalgary.ca)
