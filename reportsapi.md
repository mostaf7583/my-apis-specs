### API Specification: Get Perspective Layout

---

**1. API Overview**
   - **Purpose:** Retrieve the layout information of a perspective.
   - **Endpoint:** `/api/perspectives/{perspectiveName}`
   - **Method:** `GET`
   - **Description:** This API takes a perspective name as a path parameter and returns the layout information in a structured format.

---

**2. Endpoints**
   - **GET** `/api/perspectives/{perspectiveName}`

---

**3. Path Parameters**
   - `perspectiveName` (string, required): The name of the perspective you want to retrieve. This should be passed as part of the URL.

---

**4. Request Headers**
   - `Content-Type: application/json`
   - Optional: `Authorization: Bearer <token>` (if authentication is required).

---

**5. Example Request**
   - **URL:** `/api/perspectives/mostafa7583`

   - **Request Example:**
     ```http
     GET /api/perspectives/mostafa7583 HTTP/1.1
     Host: api.example.com
     Authorization: Bearer <token>  (optional)
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
                   "json": "{\n  \"uuid\": \"gwt-uid-233\",\n  \"type\": \"BARCHART\",\n  \"subtype\": \"BAR\",\n  \"general\": {\n    \"title\": \"- New Displayer -\",\n    \"visible\": \"false\"\n  },\n  \"chart\": {\n    \"width\": \"500\",\n    \"height\": \"250\",\n    \"margin\": {\n      \"top\": \"10\",\n      \"bottom\": \"40\",\n      \"left\": \"100\",\n      \"right\": \"50\"\n    },\n    \"legend\": {\n      \"show\": \"true\",\n      \"position\": \"RIGHT\"\n    }\n  },\n  \"filter\": {\n    \"enabled\": \"true\",\n    \"selfapply\": \"false\",\n    \"notification\": \"true\",\n    \"listening\": \"true\"\n  },\n  \"dataSet\": {\n    \"column.0\": {\n      \"id\": \"Country\",\n      \"type\": \"LABEL\",\n      \"values\": [\n        \"United States\",\n        \"China\",\n        \"Japan\",\n        \"Germany\",\n        \"United Kingdom\",\n        \"France\",\n        \"Brazil\"\n      ]\n    },\n    \"column.1\": {\n      \"id\": \"GDP 2013\",\n      \"type\": \"NUMBER\",\n      \"values\": [\n        \"16768100\",\n        \"9240270\",\n        \"4919563\",\n        \"3730261\",\n        \"2678455\",\n        \"2806428\",\n        \"2245673\"\n      ]\n    },\n    \"column.2\": {\n      \"id\": \"GDP 2014\",\n      \"type\": \"NUMBER\",\n      \"values\": [\n        \"17418925\",\n        \"1038080\",\n        \"4616335\",\n        \"3859547\",\n        \"2945146\",\n        \"2846889\",\n        \"2353025\"\n      ]\n    }\n  },\n  \"columns\": [\n    {\n      \"id\": \"Country\",\n      \"name\": \"Country\"\n    },\n    {\n      \"id\": \"GDP 2013\",\n      \"name\": \"2013\",\n      \"pattern\": \"$ #,### M\"\n    },\n    {\n      \"id\": \"GDP 2014\",\n      \"name\": \"2014\",\n      \"pattern\": \"$ #,### M\"\n    }\n  ]\n}"
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
