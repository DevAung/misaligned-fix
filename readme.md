# Fix misaligned bubbles

![](image-1.png)

>To fix the bubbles are misaligned, copy gobi script from one of the bubble elements and place it within the `<head> ... </head>` tags of your HTML document. This single placement eliminates the need to insert the script separately into each bubble element. This streamlined approach enables the use of the Gobi story script across multiple bubbles without redundancy.

## 1. Copy the Gobi script from one of the bubble elements.
![Alt text](image-2.png)

## 2. Paste the copied Gobi script inside the `<head> ... </head>` tags of your HTML document.
![Alt text](image-3.png)
## 3. Remove all script tags inside Gobi story bubble elements.
```html
<html>
  <head>
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />

    <!-- other code  -->

    <!-- add gobi script in <head> tag -->
    <script
      src="https://unpkg.com/@gobistories/gobi-web-integration@^6"
      async=""
      onload="gobi.discover()"
    ></script>
  </head>

  <body>
    <!-- other code  -->

    <div class="uk-slider-container">
      <ul>
        <li
          class="uk-width-1-1 uk-width-1-2@s uk-width-1-3@m"
          role="tabpanel"
          aria-label="1 of 11"
          tabindex="-1"
          aria-hidden="true"
          id="uk-slider-46-item-0"
          style="order: 1"
        >
          <div class="el-item uk-panel uk-margin-remove-first-child">
            <div class="el-content uk-panel uk-margin-top">
              <!-- remove gobi script from element -->
              <div
                class="gobi-stories"
                data-gobi-stories="ucor3"
                data-gobi-color="#ec046c"
                data-gobi-bubble-size="250px"
                data-gobi-animated-bubble="true"
                data-gobi-disable-shadow-dom="false"
                data-gobi-inherit-text-font-family="true"
                data-gobi-auto-start-with-sound="true"
              ></div>
              <!-- other code -->
            </div>
            <div class="el-meta">
              SoMe-anvsarlig og leder av ungdomsredaksjon
            </div>
          </div>
        </li>
        <li
          class="uk-width-1-1 uk-width-1-2@s uk-width-1-3@m"
          role="tabpanel"
          aria-label="2 of 11"
          tabindex="-1"
          aria-hidden="true"
          id="uk-slider-46-item-1"
          style="order: 1"
        >
          <div class="el-item uk-panel uk-margin-remove-first-child">
            <div class="el-content uk-panel uk-margin-top">
              <!-- remove gobi script from element -->

              <div
                class="gobi-stories"
                data-gobi-stories="5ppbr"
                data-gobi-color="#ec0086"
                data-gobi-bubble-size="250px"
                data-gobi-animated-bubble="true"
                data-gobi-disable-shadow-dom="false"
                data-gobi-inherit-text-font-family="true"
                data-gobi-auto-start-with-sound="true"
              ></div>
              <!-- other code -->
            </div>
            <div class="el-meta">Utvikler</div>
          </div>
        </li>
        <li
          class="uk-width-1-1 uk-width-1-2@s uk-width-1-3@m"
          role="tabpanel"
          aria-label="3 of 11"
          tabindex="-1"
          aria-hidden="true"
          id="uk-slider-46-item-2"
          style="order: 1"
        >
          <div class="el-item uk-panel uk-margin-remove-first-child">
            <div class="el-content uk-panel uk-margin-top">

              <!-- remove gobi script from element -->

              <div
                class="gobi-stories"
                data-gobi-stories="p2mwp"
                data-gobi-color="#ec0086"
                data-gobi-bubble-size="250px"
                data-gobi-animated-bubble="true"
                data-gobi-disable-shadow-dom="false"
                data-gobi-inherit-text-font-family="true"
                data-gobi-auto-start-with-sound="true"
              ></div>
              <!-- other code -->
            </div>
            <div class="el-meta">Innholdsprodusent</div>
          </div>
        </li>
        <!-- more bubbles  -->
      </ul>
    </div>

    <!-- other code -->


```
## Result
![](image.png)