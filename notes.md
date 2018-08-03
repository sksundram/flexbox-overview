# Flexbox Notes

![1-main-flexbox-concepts](https://i.imgur.com/rZNhq9U.png)

---

![2-flexbox-properties-overview](https://i.imgur.com/LYNwuNJ.png)

---

## FLEX CONTAINER


1. `flex-direction` -> direction of the **main-axis**
2. `flex-direction:` - **row**, row-reverse, column, column-reverse

---

3. `justify-content` -> how the flex items are aligned along the **main-axis**
4. `justify-content:` - **flex-start**, flex-end, center, space-around, space-between, space-evenly

---

5. `align-items` -> how the flex items are aligned along the **cross-axis**
6. `align-items` - **stretch**, center, flex-start, flex-end, baseline

> **stretch** stretches all other elements to match the height of the highest flex-item

> **baseline** aligns texts on the flex-items along a line

---

## FLEX ITEMS

1. `align-self` -> **overrides** `align-items` property for one individual item
2. `align-self` - **stretch**, center, flex-start, flex-end, baseline

---

3. `order` -> to **rearrange** flex-items to one'choice
4. `order` - **0**, any integer

---
5. `flex-grow` -> ability of a flex-item to grow (to capture all the available space)
6. `flex-grow` - **0**, +ve number (w.r.t another flex-item's `flex-grow` value)

---
7. `flex-shrink` -> controls how a flex-item shrinks
8. `flex-shrink` - **1** -> flex-item is allowed to shrink 

> `flex-shrink: 0` - not allowed to shrink; viewport increases to fit other elements if any

---

9. `flex-basis` -> set the width of a flex-item
10. `flex-basis` - **auto**, typical width values

---

11. `flex` -> short for (`flex-grow` `flex-shrink` `flex-basis`)

> `flex: 1` === `flex-grow: 1`

---

## What happens when there are a lot of flex-items?

At first they all will be cramped. If we decrease the browser's window, at some point, flex-items will start **overflowing** the flex-container. To counter this issue, we use **`flex-wrap`** on the **flex-container**.

12. `flex-wrap` -> creates new line(s) for flex-items not fitting in the container
13. `flex-wrap` - **nowrap**, wrap, wrap-reverse

---

14. `align-content` -> aligns the **rows** along the **cross-axis**
15. `align-content` - **stretch**, flex-start, flex-end, center, space-around, space-between
