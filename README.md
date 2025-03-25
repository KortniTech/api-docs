# api-docs
Plays API Documentation 

# Roster Upload API

**POST** `/api/rosters/import`  
Uploads a new team roster to the ScorePAD NOW system. This endpoint supports both CSV and XML file formats.

---

## 🛠️ Request Parameters

| Name       | Type   | Required | Description                                                                 |
|------------|--------|----------|-----------------------------------------------------------------------------|
| `file`     | file   | ✅        | The roster file in `.csv` or `.xml` format.                                |
| `team_id`  | string | ✅        | The unique identifier for the team.                                        |
| `league_id`| string | ✅        | The unique identifier for the league.                                      |
| `season`   | string | ❌        | The season to apply the roster to (e.g., `2025`). Defaults to current season. |

---

## 🔐 Headers

