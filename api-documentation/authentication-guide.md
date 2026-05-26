# Authentication Guide

## Overview

This document explains how to authenticate requests for the Sports Data API.

---

## Authentication Method

The API uses Bearer Token authentication.

Include the token in the request header.

## Example Header

```http
Authorization: Bearer YOUR_API_TOKEN
```

---

## Sample Request

```http
GET /v1/players
Host: api.sportsdata.com
Authorization: Bearer YOUR_API_TOKEN
```

---

## Error Responses

| Status Code | Description |
|---|---|
| 401 | Invalid token |
| 403 | Access denied |
| 500 | Internal server error |
