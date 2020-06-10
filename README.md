# Scss Helpers Library 

  Scss Helpers Lbrary is a toolkit of mixins and classes designated to help you to style your SCSS;

  
    
      
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
    @import '~@luaguillande/scss_helpers/_paddings';
    @import '~@luaguillande/scss_helpers/_margins';
  ```

  2.2 Or import all the files

  ```bash
      @import '~@luaguillande/scss_helpers/all';
  ```

## 3 Set your colors

  Set the theme in `app.scss`. You also can create new class names by changing the variable name.

  ```bash
    @include syntax-colors(
        $primary:  #F9CD16,
        $secondary: #3C3C3B,
        $error: #ff5d48,
        $white: #ffffff,
        $black: #000000,
        $info: #818181,
        $softgrey: #EDEDED,
    )
  ```

## 4 Use the classes in your html

  ```bash
    <div class="primary-text secondary pa-5 mx-10 my-3">My Div</div>
  ```
<br><br>

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
  
  You also can create new class names by changing the variable name.

  ```bash
    @include syntax-colors(
        $primary:  #F9CD16,
        $secondary: #3C3C3B,
        $error: #ff5d48,
        $white: #ffffff,
        $black: #000000,
        $info: #818181,
        $softgrey: #EDEDED,
    )
  ```

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
  

## Enjoy.

  @luaguillande - 31solutions.com