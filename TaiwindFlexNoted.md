# walkthrough of key Tailwind CSS utility classes
flex, padding (p-4), margins, and alignment — so you understand how they control layout and spacing.

## 🔧 1. flex – Making Flexbox Layouts
Basic Example
```html
<div class="flex">
  <div class="bg-red-200 p-4">Box 1</div>
  <div class="bg-blue-200 p-4">Box 2</div>
</div>
```
🔍 What it does:
flex turns the container into a flexbox, laying out children horizontally by default.
Each child becomes a flex item.
You can change direction, alignment, and spacing easily.

## 🔄 2. flex-row vs flex-col
```html
<div class="flex flex-col">
  <div class="bg-red-200 p-4">Top</div>
  <div class="bg-blue-200 p-4">Bottom</div>
</div>
```
flex-row (default): horizontal layout
flex-col: vertical layout

## 🎯 3. Justify & Align Items
```html
<div class="flex justify-between items-center h-32 bg-gray-100 p-4">
  <div class="bg-red-300 p-2">Left</div>
  <div class="bg-blue-300 p-2">Right</div>
</div>
```
🔍 Explanation:
justify-between: pushes children apart horizontally

items-center: aligns children vertically to the center

h-32: sets a fixed height so you can see vertical alignment

p-4: adds inner space (padding) around content inside the container

## 📦 4. Padding and Margin
Padding (p-*) – space inside an element
p-4: padding on all sides

pt-4: padding top

px-4: padding left & right

py-4: padding top & bottom

```html
<div class="bg-yellow-100 p-4">Padded Box</div>
```
Margin (m-*) – space outside an element
m-4: margin on all sides

mt-4: margin top

mx-4: margin left & right

mb-2: margin bottom

```html
<div class="bg-green-200 m-4">Box with margin</div>
```
## 💡 Bonus: Gap (space between flex items)
```html
<div class="flex gap-4">
  <div class="bg-pink-200 p-4">Box A</div>
  <div class="bg-pink-300 p-4">Box B</div>
</div>
```
gap-4: adds spacing between the flex items (like margin but cleaner)
