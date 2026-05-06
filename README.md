# Integrated Chatbot App 🍔🤖

A comprehensive, Java Swing-based food ordering platform that bridges the gap between buyers and multiple sellers through an intuitive, real-time chat-based interface.

## 🌟 Key Features

### 🛒 Buyer Experience
- **Natural Language Ordering**: Type queries like "I want something spicy" or "Cari nasi padang yang murah".
- **Synonym Engine**: Supports Indonesian keywords (e.g., *pedas* for spicy, *es* for cold, *murah* for cheap) to understand user intent.
- **Recommendations & Offers**: Receive automated store recommendations and special combo offers directly in the chat.
- **Multi-Seller Cart**: Add items from different stores into a single cart and checkout seamlessly.
- **Real-Time Tracking**: Monitor order status updates as they happen.
- **Interactive Delivery Map**: Visualize the delivery route from the restaurant to your location using custom `Graphics2D` rendering.

### 🏪 Seller Experience
- **Merchant Dashboard**: Each store manages its own orders and interactions.
- **Private Messaging**: Direct communication channel between buyers and sellers for specific queries.
- **Order Management**: Sellers can Accept, Process, and Dispatch orders, with real-time status synchronization.
- **Availability Toggle**: Sellers can set their status to "Busy" to automatically adjust buyer wait times.

## 🛠️ Technologies Used

- **Language**: Java
- **GUI Framework**: Java Swing & AWT
- **Graphics**: Custom `Graphics2D` for interactive maps
- **Design Patterns**: 
  - **Observer Pattern**: Ensures UI components stay synchronized with backend state changes (e.g., status updates).
  - **Bridge Pattern**: Facilitates communication between different system components.
- **Data Structures**: Enums for Categories and Order Status to maintain clean, type-safe code.

## 📂 Project Structure

- **`IntegratedChatbotApp.java`**: The primary source file containing the entire application logic, including:
  - `MultiStoreSystem`: Logic for managing sellers, menus, and search.
  - `ChatBridge`: Communication hub between buyers and sellers.
  - `BuyerChatWindow` & `SellerWindow`: UI components for the respective roles.
  - `Order`, `ShoppingCart`, & `MenuItem`: Core data models.
  - `SimpleMapWindow` & `MapCanvas`: Delivery visualization components.
- **`explain.txt`**: A project presentation guide and demo script.

## 🚀 How to Run

1.  **Prerequisites**: Ensure you have the Java Development Kit (JDK) installed on your system.
2.  **Compile**: Open your terminal/command prompt in the project directory and run:
    ```bash
    javac *.java
    ```
3.  **Launch**: Run the main application:
    ```bash
    java IntegratedChatbotApp
    ```

## 📝 Demo Flow

1.  **Search**: Type "pedas" in the chatbot to see spicy food suggestions.
2.  **Add to Cart**: Click "Add to Cart" on any recommended item.
3.  **Checkout**: Go to the **🛒 Cart** tab and complete the checkout process.
4.  **Merchant View**: The Seller Window will appear. Click **Accept Order** → **On Process**.
5.  **Status Sync**: Observe the status changing in the Buyer Window automatically.
6.  **Track**: Click **📍 View Map** to see the interactive delivery route.
7.  **Complete**: Finalize the order in the Seller Window and check the **📜 History** tab.

---
*Developed as a demonstration of Java Swing capabilities and modern design patterns in e-commerce applications.*
