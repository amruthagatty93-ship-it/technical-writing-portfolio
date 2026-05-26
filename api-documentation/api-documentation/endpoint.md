# Player Statistics Endpoint

## Endpoint

```http
GET /v1/player/stats
```

---

## Description

Returns player statistics for a selected season.

---

## Query Parameters

| Parameter | Type | Required | Description |
|---|---|---|---|
| player_id | integer | Yes | Unique player ID |
| season | string | Yes | Season year |

---

## Sample Request

```http
GET /v1/player/stats?player_id=1001&season=2025
```

---

## Sample Response

```json
{
  "player_id": 1001,
  "season": "2025",
  "games_played": 82,
  "runs": 95,
  "hits": 140
}
```

---

## Error Codes

| Code | Description |
|---|---|
| 400 | Invalid request |
| 404 | Player not found |
| 500 | Server error |
