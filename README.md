# Greeting Cards Template

This is a simple React application that dynamically displays greeting cards using React components. The cards display a greeting message along with a name, both passed as props. The application uses basic React and JSX to render the content, and it's styled with simple CSS.

## Project Structure

The main components in this project are:

1. **GreetingCard Component**: This is a stateless functional component that accepts two props (`greeting` and `name`) and renders a card-like UI displaying the provided greeting and name.
2. **App Component**: The main component that holds an array of objects, each containing a greeting and a name. It maps over this array and renders multiple `GreetingCard` components.

## How It Works

- **GreetingCard Component**:

  - This component is responsible for rendering individual greeting cards.
  - It takes in two props:
    - `greeting`: The message to be displayed (e.g., "Hello").
    - `name`: The name of the person to be greeted (e.g., "John").
  - These props are displayed in two `<h2>` and `<h3>` tags.

- **App Component**:
  - This component contains an array called `subject`, which is a list of objects. Each object has two properties: `greeting` and `name`.
  - The array is mapped over, and for each item, a `GreetingCard` component is rendered by passing the `greeting` and `name` as props.
  - The cards are displayed inside a `.container` div, which is styled using Flexbox for a clean, centered layout.

## Styling

- **Flexbox Layout**:

  - The `.container` class uses Flexbox to display the greeting cards side by side, ensuring they are evenly spaced on the page.

- **Card Style**:
  - The `.card` class styles each individual card with a border, background color, and rounded corners for a clean and visually appealing layout.

## How to Use

1. **Running the Application**:

   - To run this code, simply copy it into an HTML file, and include the React, ReactDOM, and Babel CDN links as shown.
   - Open the file in your browser, and it will render three greeting cards with different messages.

2. **Customizing the Greeting Cards**:
   - You can add or modify the greeting messages by updating the `subject` array in the `App` component.
   - For example, you can add new objects with different greetings and names to render more cards.
