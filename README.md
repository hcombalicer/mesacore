# mesacore
The unified API and AI Agent for structured recipes, allergen-safe cooking, and macro-optimized meal planning. From Filipino classics to global diets.

## 🚀 The Mission
Generic AI tools often suggest impractical recipes or ignore life-critical allergen constraints. **MesaCore** provides a "Grounded" data layer. It allows AI Agents to query a verified database for recipes based on ingredients-on-hand, dietary restrictions, and specific caloric targets.

## 🛠️ Tech Stack
*   **Language:** Python (FastAPI)
*   **Infrastructure:** Google Cloud Platform (GCP)
*   **Database:** Firestore (NoSQL)
*   **AI Orchestration:** TBD
*   **Auth:** TBD

## 📋 Target Features
- [ ] **Phase 1: The Engine**
    - Free API service hosted on GCP.
    - Structured Recipe Schema: Ingredients, Instructions, Calories, and Video links.
    - RAG-enabled AI Agent for recipe recommendations.
    - Secure Admin endpoints for database management.
- [ ] **Phase 2: Personalization**
    - User profiles with Persistent Allergen Filtering.
    - Google Social Login integration.
    - Meal Plan Generator based on ingredient availability.
- [ ] **Phase 3: Health Hub**
    - Precise Calorie and Macro tracking.
    - Dynamic Diet Plans (e.g., High Protein, Keto).

## 🧬 Recipe Schema Example
MesaCore uses a highly structured JSON format to ensure AI agents can parse instructions step-by-step:

```json
{
  "name": "Chicken Adobo",
  "diet_tags": ["Keto", "High-Protein"],
  "allergens": ["Soy"],
  "instructions": [
    {
      "step": 1,
      "action": "Marinate",
      "description": "Combine chicken and soy sauce..."
    }
  ]
}
