# Rebuild Mobile Website UI - HomeHunts

## Goal
This project involves rebuilding the HomeHunts page of Furrl's mobile website, implementing specific functionalities, and hosting the page. The final product is hosted at [https://furrl-website.netlify.app/](https://furrl-website.netlify.app/).
**Github Repo** : https://github.com/hkumariitr/psychic-doodle

## Features Implemented
### Top Navigation Bar
- **Wishlist Button**: Redirects to Furrl Wishlist.
- **Cart Button**: Redirects to the Furrl Cart.

### Product List
- **Infinite Scroll**: The page initially renders with a set of products and fetches more as the user scrolls.
- **Product Click**: Redirects to the corresponding product details page.
- **Share Button**: Opens a generic share component containing the link to the product detail page.

### Technical Requirements
- **Framework**: React.js
- **Language**: Javascript (optional, not used in the provided code)
- **Libraries**: React-icons

## File Structure

# Home.js Overview
The `Home.js` file is the main component of the HomeHunts page. It fetches product data, vibe details, and filters from the Furrl API and handles infinite scrolling for loading more products.

### Code Breakdown

#### State Variables
- **productsList**: Array storing the list of products.
- **totalProducts**: Number of total products.
- **filtersList**: Array storing the list of filters.
- **vibeDetails**: Object storing the details of the vibe.
- **pageNumber**: Current page number for infinite scroll.
- **error**: Stores any error encountered during API calls.
- **loading**: Boolean indicating if the data is currently being fetched.

#### API Calls
- **getProducts**: Fetches products for the current page.
- **getVibe**: Fetches details of the vibe.
- **getFilters**: Fetches filters for the products.

#### Infinite Scroll
The `handleInfiniteScroll` function increments the page number when the user scrolls to the bottom of the page.

#### useEffect Hooks
- **Initial Render**: Fetches vibe details and filters, and sets up the scroll event listener.
- **Page Number Change**: Fetches more products whenever the page number changes.

### Components Used
- **BannerSection**: Displays vibe details.
- **FiltersSection**: Displays filters.
- **ProductsSection**: Displays the list of products.
- **Loader**: Displays a loading indicator.

## Hosting
The project is hosted on Netlify. You can access it here: https://furrl-website.netlify.app/.

## Conclusion
This project demonstrates the ability to rebuild a mobile webpage with dynamic data fetching and infinite scrolling. The use of React functional components and hooks ensures a modern and efficient implementation. The final product meets the specified requirements and is hosted for easy access and demonstration.
