# rn-assignment6-11011472
 
Introduction
This project is a React Native application designed to simulate an e-commerce shopping cart experience. Users can browse products, add them to their cart, and manage their cart items. The application uses AsyncStorage to save the cart state locally, ensuring that the cart contents persist across app sessions.

Features
Product Listing Screen: Shows a list of available products with options to add them to the cart.
Cart Screen: Displays items added to the cart and provides options to remove them.
Add to Cart: Each product on the product listing screen has an "Add to Cart" button.
Remove from Cart: Each item on the cart screen has a "Remove" button.
Local Storage: Cart items are stored locally using AsyncStorage to maintain state between sessions.

Design and Functionality
UI Design
The user interface is designed for simplicity and ease of use:

Product Listing Screen: Displays each product with its image, name, price, and an "Add to Cart" button in a clean, organized layout.
Cart Screen: Lists the products added to the cart with an option to remove each item and displays the total price.
Navigation: Users can easily navigate between the product listing and cart screens using header buttons.

Data Storage
AsyncStorage: Chosen for its simplicity in handling JSON data and providing persistent local storage. It ensures that the cart's state is maintained between app sessions.

Component Structure
HomeScreen.js:
Displays the list of products.
Utilizes the ProductItem component for rendering individual products.
Manages adding products to the cart and storing them in AsyncStorage.

CartScreen.js:
Retrieves and displays cart items from AsyncStorage.
Uses the CartItem component for rendering individual cart items.
Manages removing products from the cart and updating AsyncStorage.

ProductItem.js:
A reusable component for displaying product details on the HomeScreen.
Includes product image, name, price, and an "Add to Cart" button.

CartItem.js:
A reusable component for displaying cart item details on the CartScreen.
Includes product name, price, and a "Remove" button.

State Management
React's useState and useEffect hooks are used to manage the application state.
The cart items are stored and managed locally within each component and synchronized with AsyncStorage for persistence.

Implementation
Key Components

HomeScreen.js:
Displays products in a scrollable list.
Uses ProductItem for each product.
Handles adding products to the cart and saving them in AsyncStorage.

CartScreen.js:
Displays cart items fetched from AsyncStorage.
Uses CartItem for each cart item.
Handles removing products from the cart and updating AsyncStorage.

ProductItem.js:
Renders individual product details and includes an "Add to Cart" button.

CartItem.js:
Renders individual cart item details and includes a "Remove" button.

Screenshots
Home Screen
![SCREENSHOT1](<myapp/assets/SCREENSHOT1.png>)
![SCREENSHOT2](<myapp/assets/SCREENSHOT2.png>)

Cart Screen
![SCREENSHOT3](<myapp/assets/SCREENSHOT3.png>)

Conclusion
This React Native shopping cart application offers a straightforward and user-friendly shopping experience. The use of AsyncStorage ensures that the cart's state is preserved between sessions, providing a seamless user experience. The modular design of the components allows for easy scalability and maintenance, making it a robust solution for mobile e-commerce applications.