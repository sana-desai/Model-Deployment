# SuperKart Sales Forecasting – XGBoost Deployment Project 🚀

## 📌 Business Context  
Sales forecasting is essential for supermarket chains like **SuperKart**, operating across diverse city tiers. Accurate predictions enable:  
- Optimized **inventory planning**  
- Smarter **regional growth strategies**  
- Improved **supply chain efficiency**  
- Reliable **financial forecasting & investor reporting**  

Traditional planning based on intuition or outdated systems can be error-prone. To overcome this, SuperKart collaborated with a data science team to build a robust ML-powered forecasting solution, fully deployable to production.  

---

## 🎯 Objective  
Develop and deploy a machine learning model that:  
- Predicts **`Product_Store_Sales_Total`**  
- Generalizes well to unseen/new data  
- Integrates seamlessly into SuperKart’s systems via **Hugging Face Spaces** (frontend + backend)  

---

## 📊 Dataset Overview  
The dataset contains product-level sales data across stores with numerical & categorical features.  

| Feature | Description |
|---------|-------------|
| `Product_Id` | Unique product identifier |
| `Product_Weight` | Weight of the product |
| `Product_Sugar_Content` | Sugar content (Low, Regular, No sugar) |
| `Product_Allocated_Area` | Share of store’s display area |
| `Product_Type` | Category of product (e.g., Dairy, Meat, Snacks) |
| `Product_MRP` | Maximum Retail Price |
| `Store_Id` | Unique store identifier |
| `Store_Establishment_Year` | Year store was opened |
| `Store_Size` | Store size (High, Medium, Low) |
| `Store_Location_City_Type` | Tier 1 / Tier 2 / Tier 3 |
| `Store_Type` | Store format (Departmental, Supermarket, etc.) |
| **Target**: `Product_Store_Sales_Total` | Total product sales in that store |

---

## 🛠️ Technologies & Tools  
- **Programming**: Python  
- **Modeling**: XGBoost, Random Forest, Linear Regression  
- **Evaluation**: RMSE, MAPE, R² Score  
- **Preprocessing**: One-Hot Encoding, Standard Scaling  
- **Deployment**: Hugging Face Spaces  
- **Frontend**: Streamlit  
- **Backend**: FastAPI (with Inference API)  
- **DevOps**: Docker, GitHub Actions (CI/CD)  

---

## 📈 Key Insights & Results  
- **Tuned XGBoost** achieved **~93% R²** on train/test sets → strong generalization  
- **Top predictors**: Product_MRP, Product_Allocated_Area, Store_Age, Product_Weight  
- **Model performance**:  
  - RMSE = **283.12**  
  - MAPE = **4.2%**  
- Random Forest tended to overfit, while XGBoost provided better reliability  

---

## 💡 Business Recommendations  
- **Dynamic Pricing** → Adjust prices by location/season using forecast trends  
- **Smart Inventory Allocation** → Restock high-sale products with larger display areas  
- **Store Expansion** → Focus on Tier-2 cities with medium-sized formats  
- **Promotional Campaigns** → Tailor by product type for higher ROI  
- **Investor Reports** → Use forecasts to simulate profits and report financial health  
- **Customer Segmentation** → Combine forecasts with customer data for targeted marketing  

---

## 🚀 Deployment  
- **Frontend** → Streamlit App  
- **Backend** → FastAPI Inference Endpoint  
- **Platform** → Hugging Face Spaces (live deployment)  

---

## 📂 Project Structure  
