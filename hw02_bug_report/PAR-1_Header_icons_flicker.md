### **Bug Report PAR-1: Header icons flicker

**Title:** Visual flicker on header icons due to lack of asset preloading
**Environment:** All Browsers (Chrome, Firefox, Safari)

**Description:**
There is a noticeable delay before hover-state images appear on navigation icons. This causes the icon to disappear or flicker briefly while the browser fetches the new image from the server.

**Steps to Reproduce:**
1. Clear browser cache.
2. Navigate to the ParaBank homepage.
3. Hover the mouse cursor over the **Home** (house) icon.
4. Observe the momentary "gap" or flicker.

**Expected Result:**
The hover state should trigger instantly with no visual lag.

**Actual Result:**
The UI flickers because the browser initiates a network request for the hover image only upon user interaction.

