# AIM :
## To interpret the functionalities of media queries in html and css.
# Objective 1 :
### Using CSS media queries to modify the webpage's color scheme.
## Code :
```
<html>
<!DOCTYPE.html>
<head>
</head>
<style>
    /* Default Color Scheme */
body {
  background-color: #f4f4f4;
  color: #333;
}

a {
  color: #007bff;
}

/* Small Screen Adaptation */
@media (max-width: 600px) {
  body {
    background-color: #333;
    color: #f4f4f4;
  }

  a {
    color: #28a745;
  }
}

/* Dark Mode Preference */
@media (prefers-color-scheme: dark) {
  body {
    background-color: #000;
    color: #fff;
  }

  a {
    color: #17a2b8;
  }
}

</style>

<body>
<p>This is my Webpage</p>
<a href="saveetha.ac.in">SAVEETHA WEBSITE</a>
</body>
</html>
```
# Output :
### Webpage's color scheme when it is on larger devices like pcs and desktops.


![Screenshot 2023-12-13 113928](https://github.com/Madhavareddy09/ODD2023-WT-Ex-07-CSS/assets/145742470/297f81f8-8c96-4b2e-afbe-83439a54df7a)



### Webpage's color scheme when it is on smaller screens like potrait.


![image](https://github.com/Madhavareddy09/ODD2023-WT-Ex-07-CSS/assets/145742470/b8449ed7-59d1-4143-ba6d-3aad2c4365d4)

# Objective 2 :
### Using CSS media queries to modify mobile and desktop styles.
## Code :
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style type="text/css">
    /* Styles for desktop devices */
    body {
      font-size: 16px;
      background-color: #f2f2f2;
      color: #333;
    }

    .container {
      max-width: 960px;
      margin: 0 auto;
      padding: 20px;
      background-color: #fff;
      border: 1px solid #ddd;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }

    /* Media query for mobile devices with width less than 600px */
    @media screen and (max-width: 599px) {
      body {
        font-size: 14px;
        background-color: #e6e6e6;
        color: #555;
      }

      .container {
        padding: 10px;
        background-color: #f9f9f9;
        border: 1px solid #ccc;
        box-shadow: none;
      }

      .device-specific {
        font-weight: bold;
        color: #ff5733;
      }
    }
  </style>
  <title>Media Queries 2</title>
</head>
<body>
  <div class="container">
    <h1>Responsive Blog Post</h1>
    <p>This blog post content is designed to be readable on all devices. The background color and font size adjust based on the screen width.</p>
    <p class="device-specific">Important information is highlighted with bold text and a different color on mobile devices.</p>
  </div>
</body>
</html>
```
# Output :
## Webpage Design when opened on large width devices like pc
![image](https://github.com/Madhavareddy09/ODD2023-WT-Ex-07-CSS/assets/145742470/0bd60b25-1326-4ef2-bd5f-225714986eea)


## Webpage Design when opened on small width devices like mobile phones
![WhatsApp Image 2023-12-13 at 18 22 47_d66b64e3](https://github.com/Madhavareddy09/ODD2023-WT-Ex-07-CSS/assets/145742470/1d77c280-b2d4-4a95-89aa-846e964de500)


# Objective 3 :
### Using CSS media queries to represent orientation scheme.
## Code :
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Media Queries 3</title>
  <style>
    /* Styles for portrait orientation */
    @media (orientation: portrait) {
      body {
        background-color: #e6f7ff; /* Light blue background for portrait orientation */
      }
    }
    /* Styles for landscape orientation */
    @media (orientation: landscape) {
      body {
        background-color: rebeccapurple; /* Deep purple background for landscape orientation */
      }
    }
  </style>
</head>
<body>
  <h1>Webpage orientation using css media queries</h1>
  <p>this webpage is visible in purple colour on laptop and in light green when opened on smart phone</p>
</body>
</html>
```
# Output :
## Webpage's background colour is purple when opened on landscape orientation (pc)
![image](https://github.com/Madhavareddy09/ODD2023-WT-Ex-07-CSS/assets/145742470/5103ed9b-d361-4e8d-a976-21c9423c033b)

## Webpage's background colour changes to light green when opened on portriat orientation
![WhatsApp Image 2023-12-13 at 18 27 37_a46234cf](https://github.com/Madhavareddy09/ODD2023-WT-Ex-07-CSS/assets/145742470/c1f98a6e-529f-4822-afe9-bdb34b1fd2cb)

# Objective 4 :
## Responsive Typography using CSS Media queries
# Code :
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style type="text/css">
    /* Default styles for all devices */
    body {
      font-size: 16px;
      line-height: 1.6;
      margin: 20px;
    }

    /* Media query for devices with width between 600px and 899px */
    @media screen and (min-width: 600px) and (max-width: 899px) {
      body {
        font-size: 18px;
        line-height: 1.5;
      }
    }

    /* Media query for devices with width 900px and above */
    @media screen and (min-width: 900px) {
      body {
        font-size: 20px;
        line-height: 1.4;
      }
    }
  </style>
  <title>Media Queries 4</title>
</head>
<body>
<p>Font size and line height adapt to provide an optimal reading experience on devices of all sizes when we use media queries in css</p>
</body>
</html>
```
# Output :

## Font size is 18px and line height is 1.6 when opened on larger devices like pc

![image](https://github.com/Madhavareddy09/ODD2023-WT-Ex-07-CSS/assets/145742470/f516903d-5e64-4fb0-82f2-bcd1394cab1f)


## Font size is reduced to 14px on devices with a maximum width of 600px like mobile phones 

![WhatsApp Image 2023-12-13 at 18 29 53_8da3d03f](https://github.com/Madhavareddy09/ODD2023-WT-Ex-07-CSS/assets/145742470/38ccea1f-d1d8-4142-8a2a-e3d0a1f56d3f)


# Objective 5 :
## Print-friendly styles for web pages using CSS media quries
## Code :
```
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Media Queries 5</title>
  <style>
    /* Default styles for the webpage */
    body {
      background-color: #f4f4f4; /* Light gray background */
      color: #333; /* Dark gray text color */
    }

    a {
      color: #007bff; /* Blue link color */
    }

    .non-essential {
      display: block; /* Visible by default */
    }

    /* Media query for print styles */
    @media print {
      body {
        background-color: #fff; /* White background for printing */
        color: #000; /* Black text color for printing */
      }

      a {
        color: #17a2b8; /* Cyan link color for printing */
      }

      .non-essential {
        display: none; /* Hide non-essential elements for printing */
      }
    }
  </style>
</head>

<body>
  <p>We can Use the print-friendly version for a clean and efficient printout using media queries for print mode</p>
  <p class="non-essential">All the non essential elements will not be displayed when used media queries</p>
</body>

</html>
```
# Output :
## Webpage Design when opened in view-mode
![image](https://github.com/Madhavareddy09/ODD2023-WT-Ex-07-CSS/assets/145742470/b63ac5ac-9696-467e-9e69-ac54fa492596)

## Webpage Design changes when opened in print-mode
![image](https://github.com/Madhavareddy09/ODD2023-WT-Ex-07-CSS/assets/145742470/5173dbd2-ddcc-4d61-bbd5-238a47d32e27)


## Non-essential elements are not displayed in print-mode

# Objective 6 :
## Dark mode Implementation using CSS media queries

# Code :
```
<!DOCTYPE html>
<html>
<head>
</head>
<style>
/* Default Color Scheme */
body {
  background-color: #f4f4f4;
  color: #333;
}

/* Dark Mode Preference */
@media (prefers-color-scheme: dark) {
  body {
    background-color: #000;
    color: #fff;
  }
}

</style>
<body>
<p>This webpage is visible in light mode if your device is set to light theme</p>

<p>This webpage is visible in Dark mode if your device is set to Dark theme</p>

</body>
</html>
```
## Webpage is Displayed in light mode when device is running on light theme
![image](https://github.com/Madhavareddy09/ODD2023-WT-Ex-07-CSS/assets/145742470/ce218e1a-55db-42df-87d6-55e4d3ef3a15)


## Webpage is Displayed in dark mode when deivce is running on dark mode
![image](https://github.com/Madhavareddy09/ODD2023-WT-Ex-07-CSS/assets/145742470/d1dadeb1-20c8-422a-b680-506462195471)


# Result :
## Therefore, functionalities of CSS media queries are clearly demonstrated using examples for each type.

## Developed By : K.Madhava Reddy
## Register Number : 212223240064
