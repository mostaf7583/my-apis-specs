### API Specification: Get Perspective Layout

---

**1. API Overview**
   - **Purpose:** Retrieve the layout information of a perspective.
   - **Endpoint:** `/perspectives/{perspectiveName}`
   - **Method:** `GET`
   - **Description:** This API takes a perspective name as a path parameter and returns the layout information in a structured format.

---

**2. Endpoints**
   - **GET** `/perspectives/{perspectiveName}`

---

**3. Path Parameters**
   - `perspectiveName` (string, required): The name of the perspective you want to retrieve. This should be passed as part of the URL.

---

**4. Request Headers**
   - `Content-Type: application/json`
   - `Authorization: Basic'.

---

**5. Example Request**
   - **URL:** `/api/perspectives/mostafa7583`

   - **Request Example:**
     ```http
     GET /api/perspectives/mostafa7583 HTTP/1.1
     `Authorization: Basic'.
     ```

---

**6. Response Format**

   The response is a JSON object that contains the layout information of the perspective.

   ```json
   {
     "version": 3,
     "name": "mostafa7583",
     "style": "FLUID",
     "layoutProperties": {},
     "rows": [
       {
         "height": "12",
         "properties": {},
         "layoutColumns": [
           {
             "span": "12",
             "height": "12",
             "properties": {},
             "rows": [],
             "layoutComponents": [
               {
                 "dragTypeName": "org.uberfire.ext.plugin.client.perspective.editor.layout.editor.TargetDivDragComponent",
                 "properties": {
                   "ID_PARAMETER": "3403774"
                 },
                 "parts": []
               }
             ]
           }
         ]
       },
       {
         "height": "12",
         "properties": {},
         "layoutColumns": [
           {
             "span": "12",
             "height": "12",
             "properties": {},
             "rows": [],
             "layoutComponents": [
               {
                 "dragTypeName": "org.dashbuilder.client.editor.BarChartDragComponent",
                 "properties": {
                   "json": "{..}"
                 },
                 "parts": []
               }
             ]
           }
         ]
       }
     ]
   }
   ```

---

**7. Response Codes**
   - `200 OK`: Successfully retrieved the layout for the given perspective.
   - `404 Not Found`: The perspective with the specified name does not exist.
   - `500 Internal Server Error`: General server error.

---

**8. Example Response**
   ```json
   {
     "version": 3,
     "name": "mostafa7583",
     "style": "FLUID",
     "layoutProperties": {},
     "rows": [
       {
         "height": "12",
         "properties": {},
         "layoutColumns": [
           {
             "span": "12",
             "height": "12",
             "properties": {},
             "rows": [],
             "layoutComponents": [
               {
                 "dragTypeName": "org.uberfire.ext.plugin.client.perspective.editor.layout.editor.TargetDivDragComponent",
                 "properties": {
                   "ID_PARAMETER": "3403774"
                 },
                 "parts": []
               }
             ]
           }
         ]
       },
       {
         "height": "12",
         "properties": {},
         "layoutColumns": [
           {
             "span": "12",
             "height": "12",
             "properties": {},
             "rows": [],
             "layoutComponents": [
               {
                 "dragTypeName": "org.dashbuilder.client.editor.BarChartDragComponent",
                 "properties": {
                   "json": "{...}"
                 },
                 "parts": []
               }
             ]
           }
         ]
       }
     ]
   }
   ```

---
