# Printing, Combining, and Accessing Data From Indexed and Associative Arrays

A small PHP project that demonstrates indexed and associative arrays.

## What it does

- Creates an indexed array: `225, Dreams, Glass, 30, 25, 1, Globe`
- Creates an associative array: `'0' => 'Couch', 'Ice' => 'India', '6' => 'Box', 'Trip' => 'Range'`
- Prints both arrays completely as tables
- Combines them with `array_merge()` and prints the combined array
- Displays the 3rd value of the indexed array (**Glass**)
- Displays the value for the key `Ice` from the associative array (**India**)

## Files

| File | Purpose |
|---|---|
| `index.php` | PHP source code (run locally with `php -S localhost:8000`) |
| `index.html` | Static copy of the PHP output, served by GitHub Pages |
| `style.css` | Responsive styling |

## Note on GitHub Pages

GitHub Pages cannot execute PHP, so `index.html` is a pre-rendered copy of the output of `index.php`.

## Why `array_merge()` and not `+`

The keys `'0'` and `'6'` become integers in PHP and would collide with indexes 0 and 6 of the indexed array. The `+` operator would drop `Couch` and `Box`; `array_merge()` keeps all values.

## Live page

Add your GitHub Pages link here: `https://<your-username>.github.io/<repo-name>/`
