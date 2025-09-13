# dog-api-docs
API documentation work sample

# Dog Catagories API Documentation

This project demonstrates clean, standards-driven API documentation using the public Dog CEO API. It covers three endpoints with sample requests, responses, error codes, and parameter tables—ideal for showcasing technical writing and API literacy.

**Skills Highlighted:**  
- RESTful API structure  
- Markdown formatting  
- Curl usage and JSON parsing  
- Parameter and error handling documentation  
- Developer-first clarity and structure

![Markdown](https://img.shields.io/badge/Markdown-Expert-blue)

[View My GitHub Portfolio](https://github.com/malaysinghchouhan)


---

## 1. Get Random Dog Image

**Method:** `GET`  
**Endpoint:** `/breeds/image/random`  
**Full URL:** `https://dog.ceo/api/breeds/image/random`

### Parameters
| Name | Type | Required | Description |
|------|------|----------|-------------|
| None | —    | —        | Returns a random dog image from any breed |

### Sample Request
```bash
curl https://dog.ceo/api/breeds/image/random
```
### Sample Response
```json
{
  "message": [
    "https://images.dog.ceo/breeds/hound-afghan/n02088094_1003.jpg",
    "https://images.dog.ceo/breeds/hound-afghan/n02088094_1023.jpg"
    // ...more image URLs
  ],
  "status": "success"
}
```
## Error Codes
| Code | Meaning | 
|------|------|
| 200 | Success |
| 404 | Endpoint not found |
---
## 2. List All Dog Breeds

**Method:** `GET`  
**Endpoint:** `/breeds/list/all`  
**Full URL:** `https://dog.ceo/api/breeds/list/all`

### Parameters
| Name | Type | Required | Description |
|------|------|----------|-------------|
| None | —    | —        | Returns a dictionary of all dog breeds available in the API |

### Sample Request
```bash
curl https://dog.ceo/api/breeds/list/all
```
### Sample Response
```json

{
  "message": {
    "affenpinscher": [],
    "african": [],
    "airedale": [],
    "akita": [],
    "appenzeller": [],
    "australian": ["shepherd"],
    "basenji": [],
    "beagle": [],
    "bluetick": [],
    "borzoi": [],
    "bouvier": [],
    "boxer": [],
    "brabancon": [],
    "briard": [],
    "bulldog": ["boston", "english", "french"],
    "bullterrier": ["staffordshire"],
    "cairn": [],
    "cattledog": ["australian"],
    ...
  },
  "status": "success"
}
```
## Error Codes
| Code | Meaning | 
|------|------|
| 200 | Success |
| 404 | Endpoint not found |

---


## 3. Get Images by Breed

**Method:** `GET`  
**Endpoint:** `/breed/{breed-name}/images`  
**Example URL:** `https://dog.ceo/api/breed/hound/images`

### Parameters
| Name       | Type   | Required | Description                     |
|------------|--------|----------|---------------------------------|
| breed-name | string | Yes      | The name of the dog breed (e.g., `hound`, `bulldog`) |

### Sample Request
```bash
curl https://dog.ceo/api/breed/hound/images
```
## Sample Response
```json
{
  "message": [
    "https://images.dog.ceo/breeds/hound-afghan/n02088094_1003.jpg",
    "https://images.dog.ceo/breeds/hound-afghan/n02088094_1023.jpg"
    // ...more image URLs
  ],
  "status": "success"
}
```
## Error Codes
| Code | Meaning | 
|------|------|
| 200 | Success |
| 404 | Endpoint not found |

