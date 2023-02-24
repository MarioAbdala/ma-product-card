# MA-Product-Card

This is a deploy test package I created while learning React with TypeScript. It's a pretty simple Product Card Package, using different component patterns to allow direct access to properties, styles, among other things, from the package. This project was made progressively, and as you can inspect from the GitHub repository, from the following branches I will explain.

## LazyLoad (w/ React Router v6)

One of the initial points of the application, this branch has a simple app with and LazyLoad.

## LazyLoad Nested (w/ React Router v6)

An updated version of the previous branch, now with nested routes.

## Component Extend Styles (Compound Component Pattern)

This is the first component pattern I implemented, which follows a similar workflow as Material UI or Ionic. It presents these custom components as HOCs to allow certain flexibilities I later made use of, also allowing custom styles to be added as needed.

## Component Control Props

This updated branch allows user to control properties and state of the component. This pattern is commonly used in forms (as in value, onChange, and other properties).

## Component State Initializer

Lastly, the final branch is made following the State Initializer pattern. This pattern allows a quick way for the user to access every property they have control over.

## Example

```react
import { ProductCard, ProductImage, ProductTitle, ProductButtons } from 'ma-product-card';
```

```react
<ProductCard product={product} initialValues={{count: 0, maxCount: 15}}>
    {
        ({}) => (
            <>
                <ProductImage />
                <ProductTitle />
                <ProductButtons />
            </>
        )
    }
</ProductCard>
```

## Contributing

Pull requests are welcome, anything that can help me improve the project and, most importantly, continue learning. Thank you for your time.

### Mario Abdala