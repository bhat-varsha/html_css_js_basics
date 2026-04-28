Tailwind is a CSS framework ,It helps you style your webpage quickly,Tailwind gives predefined classes (utilities)

Instead of writing CSS like this:
button {
  background-color: blue;
  padding: 10px;
}

 In Tailwind, you directly write styles inside HTML: <button class="bg-blue-500 p-2">

use of Tailwind:
✅ Faster development : No need to write separate CSS file
✅ No naming headache :No need for class names like .myButton123
✅ Responsive design easily :You can make mobile + desktop layouts easily
_________________________________________________________________
Tailwind Utility Classes (Cheat Sheet)
🎨 Colors
Code	Meaning
bg-red-500	Red background
bg-blue-500	Blue background
bg-pink-900	Dark pink background
text-white	White text
text-black	Black text
text-green-700	Dark green text
📦 Spacing (Padding & Margin)
Code	Meaning
p-4	Padding on all sides
p-6	More padding
px-4	Padding left & right
py-2	Padding top & bottom
m-2	Margin on all sides
mt-4	Margin top
mb-4	Margin bottom
📐 Size
Code	Meaning
w-full	Full width
w-1/2	Half width
h-32	Fixed height
h-screen	Full screen height
🔤 Text Styling
Code	Meaning
text-sm	Small text
text-lg	Large text
text-xl	Extra large
font-bold	Bold text
text-center	Center align text
🎯 Layout
Code	Meaning
flex	Flexbox layout
grid	Grid layout
justify-center	Center horizontally
items-center	Center vertically
🎨 Borders & Effects
Code	Meaning
rounded	Rounded corners
border	Add border
shadow	Add shadow
🖱️ Hover Effects
Code	Meaning
hover:bg-blue-700	Change bg on hover
hover:text-black	Change text on hover
_________________________________________________________________
src="https://cdn.tailwindcss.com">
this is source link which we want to donwload the tailwind script from browser
_________________________________________________________________
<body class="bg-pink-900 text-white p-6">

like this we can use tailwind css Sheet
in the above bg=background color 
text color
p=padding
_________________________________________________________________
| Category          | Tailwind Class        | CSS Equivalent                             |
| ----------------- | --------------------- | ------------------------------------------ |
| **Background**    | `bg-purple-900`       | `background-color: #581c87;`               |
|                   | `bg-gray-100`         | `background-color: #f3f4f6;`               |
|                   | `bg-blue-500`         | `background-color: #3b82f6;`               |
| **Text Color**    | `text-white`          | `color: white;`                            |
|                   | `text-black`          | `color: black;`                            |
|                   | `text-red-500`        | `color: #ef4444;`                          |
| **Font Size**     | `text-sm`             | `font-size: 14px;`                         |
|                   | `text-lg`             | `font-size: 18px;`                         |
|                   | `text-xl`             | `font-size: 20px;`                         |
| **Font Weight**   | `font-bold`           | `font-weight: bold;`                       |
|                   | `font-light`          | `font-weight: 300;`                        |
| **Text Align**    | `text-center`         | `text-align: center;`                      |
|                   | `text-left`           | `text-align: left;`                        |
| **Padding**       | `p-4`                 | `padding: 16px;`                           |
|                   | `p-6`                 | `padding: 24px;`                           |
|                   | `pt-4`                | `padding-top: 16px;`                       |
|                   | `px-4`                | `padding-left: 16px; padding-right: 16px;` |
| **Margin**        | `m-4`                 | `margin: 16px;`                            |
|                   | `mt-2`                | `margin-top: 8px;`                         |
|                   | `mx-auto`             | `margin-left: auto; margin-right: auto;`   |
| **Width**         | `w-full`              | `width: 100%;`                             |
|                   | `w-1/2`               | `width: 50%;`                              |
|                   | `w-64`                | `width: 256px;`                            |
| **Height**        | `h-10`                | `height: 40px;`                            |
|                   | `h-screen`            | `height: 100vh;`                           |
| **Border**        | `border`              | `border: 1px solid;`                       |
|                   | `border-2`            | `border-width: 2px;`                       |
|                   | `border-red-500`      | `border-color: red;`                       |
| **Border Radius** | `rounded`             | `border-radius: 4px;`                      |
|                   | `rounded-lg`          | `border-radius: 8px;`                      |
|                   | `rounded-full`        | `border-radius: 9999px;`                   |
| **Flexbox**       | `flex`                | `display: flex;`                           |
|                   | `flex-col`            | `flex-direction: column;`                  |
|                   | `justify-center`      | `justify-content: center;`                 |
|                   | `items-center`        | `align-items: center;`                     |
|                   | `gap-4`               | `gap: 16px;`                               |
| **Display**       | `hidden`              | `display: none;`                           |
|                   | `block`               | `display: block;`                          |
|                   | `inline`              | `display: inline;`                         |
| **Hover Effects** | `hover:bg-yellow-700` | `:hover { background-color: #a16207; }`    |
|                   | `hover:text-white`    | `:hover { color: white; }`                 |
| **Shadow**        | `shadow`              | `box-shadow: ...;`                         |
|                   | `shadow-lg`           | `box-shadow: larger shadow;`               |
