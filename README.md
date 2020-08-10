# Scss Helpers Library 

  Scss Helpers Lbrary is a toolkit of mixins and classes designated to help you to style your SCSS.

      
## Quick start guide
  

## 1. Add the library to your project

  ```bash
      $ npm install @luaguillande/scss_helpers
  ```

## 2. Import 

  2.1 Import as needed in `app.scss`

  ```bash
    @import '~@luaguillande/scss_helpers/_text';
    @import '~@luaguillande/scss_helpers/_colors';
    @import '~@luaguillande/scss_helpers/_flexbox';
    @import '~@luaguillande/scss_helpers/_paddings';
    @import '~@luaguillande/scss_helpers/_margins';
  ```

  2.2 Or import all the files

  ```bash
      @import '~@luaguillande/scss_helpers/all';
  ```

## 3. Set your colors

  Set the theme in `app.scss` (or the file where your are importing the library). You also can create new class names by changing the variable name.

  ```bash
    @include colors(
        $primary:  #F9CD16,
        $secondary: #3C3C3B,
        $error: #ff5d48,
        $white: #ffffff,
        $black: #000000,
        $info: #818181,
        $softgrey: #EDEDED,
    )
  ```

## 4. Use the classes in your html

  ```bash
    <div class="primary-text secondary pa-5 mx-10 my-3">My Div</div>
  ```

## 5. Classes List

## Margins and Paddings

  The Paddings and Margins are responsive and can be changed according the device

  `{property}{direction}-{device}-{size}` 
    
<br><br>

  Property | Direction | Device | Sizes
--- | --- | --- | ---
`p` for `paddings` | `pa`, `py`, `px`, `pl`, `pr`, `pt`, `pb` | nothing, `xs`, `sm`, `md`, `lg`, `xl`  | `1` to `24`
`m` for `paddings` | `ma`, `my`, `mx`, `ml`, `mr`, `mt`, `mb` | nothing, `xs`, `sm`, `md`, `lg`, `xl`  | `1` to `24` 

<br><br>
     
  Property | Media Query
--- | --- 
nothing | Aplies in all devices
`xs` | `max-width  420px`
`sm` | `max-width 800px`
`md` | `max-width 1025px`
`lg` | `max-width 1601px`
`xl` | `min-width 1601px` 

<br><br>
    
  Paddings
    

  Property | Direction
--- | --- 
`pa` | padding
`py` | padding-top and padding-bottom
`px` | padding-left and padding-right
`pl` | padding-left
`pr` | padding-right
`pt` | padding-top
`pb` | padding-bottom 

  
<br><br>
    
  Margins
    

  Property | Direction
--- | --- 
`ma` | margin
`my` | margin-top and margin-bottom
`mx` | margin-left and margin-right
`ml` | margin-left
`mr` | margin-right
`mt` | margin-top
`mb` | margin-bottom 
  
    
<br><br>
    
      

  Example:

  ```bash
    <div class="pa-10 pa-xs-2 my-lg-10">My Div</div>
  ```

## Colors

  For backgrounds: `{name}`
  For text colors: `{name}--text`

 Example:

  ```bash
    <div class="primary white--text">My Div</div>
  ```
      
  You can also use 5 lighter and darker color variables automatically generated from your theme.

  <br>

    ```bash
      <div class="primary-lighten-1--text secondary--darken-3">My Div</div>
    ```
  <br><br>


## Align Text

  Classes to help the text alignment

  Class | Property
--- | --- 
`text-left` | `text-align: left`
`text-right` | `text-align: right`
`text-center` | `text-align: center`

<br><br>

  Example:

  ```bash
    <div class="text-left">My Div</div>
  ```

## Text Transform

  Classes to change the text case

  Class | Property
--- | --- 
`text-uppercase` | `text-transform:: uppercase`
`text-lowercase` | `text-transform:: lowercase`
`text-capitalize` | `text-transform:: capitalize`

<br><br>

  Example:

  ```bash
    <div class="text-uppercase">My Div</div>
  ```
  
## Font Weight

  Classes to change the `font-weight`

  Class | Property
--- | --- 
`font-100`| `font-weight: 100`
`font-200`| `font-weight: 200`
`font-300`| `font-weight: 300`
`font-400`| `font-weight: 400`
`font-500`| `font-weight: 500`
`font-600`| `font-weight: 600`
`font-700`| `font-weight: 700`
`font-800`| `font-weight: 800`
`font-900`| `font-weight: 900`


  
## FlexBox

  Classes to help the layout with `display:flex`

<br><br>
Use the `class="flex"` to apply the `display:flex` style.


Wrapping

  Class | Property | Details
--- | --- 
`wrap` | `flex-wrap: wrap` | breaks child elements into new lines when space runs out
`no-wrap` | `flex-wrap: nowrap` | keeps child elements on the same line, even if there is no space
<br><br>
<br><br>

Vertical Align

  Class | Property | Details
--- | --- 
`align-center` | `align-items: center` | vertically centers the child element
`align-flex-end` | `align-items: flex-end` | aligns the child element at the end of the parent element
`align-stretch` | `align-items: stretch` | vertically distribute the child elements
<br><br>
<br><br>

Horizontal Align

  Class | Property | Details
--- | --- 
`justify-center` | `justify-items: center` | horizontally centers the child element
`justify-end` | `justify-items: end` | horizontally aligns the child element at the end of the parent element
`justify-space-between` | `justify-items: space-between` | horizontally distribute the child elements
`justify-space-around` | `justify-items: space-around` | horizontally distribute the child elements

<br><br>

  Example:

  ```bash
    <div class="flex wrap justify-space-around align-center">My Div</div>
  ```
  

## Enjoy!

  @luaguillande - 31solutions.com