
# react-modal-bizwi

A simple and reusable React modal component for displaying customizable modal windows.



## Installation

Install my-project with npm

```bash
  npm install react-modal-bizwi
```  
Or
```bash
  yarn add react-modal-bizwi
```


## Usage/Examples

```js
import React, { useState } from 'react';
import Modal from 'react-modal-bizwi';

const ExampleComponent = () => {
  const [isModalOpen, setIsModalOpen] = useState(false);

  return (
    <div>
      <button onClick={() => setIsModalOpen(true)}>Open Modal</button>
      <Modal isOpen={isModalOpen} onClose={() => setIsModalOpen(false)}>
        <p>Employee Created!</p>
      </Modal>
    </div>
  );
};

export default ExampleComponent;
```


## Props

The `react-modal-bizwi` component accepts the following props:

- `isOpen` (`boolean`,required): Controls whether the modal is visible.
- `onClose ` (`function`,required): Controls whether the modal is visible.
- `children  ` (`ReactNode`,required): Controls whether the modal is visible.
- `style` (`object`, optional): Inline styles to customize the modal container.
- `className` (`string`, optional): Custom class name to apply to the modal container for additional styling.


## Customization
### Using `className`

You can customize the modal's appearance by passing a custom `className` prop:

```js
<Modal isOpen={isOpen} onClose={() => setIsOpen(false)} className="custom-modal">
  <p>Customizable Content</p>
</Modal>

```
Add your styles in a CSS/SCSS file:
```css
.custom-modal {
  background-color: blue;
  padding: 20px;
  border-radius: 8px;
}
```

### Using style Prop

Alternatively, you can customize styles using the `style` prop:

```js
<Modal isOpen={isOpen} onClose={() => setIsOpen(false)} style={{ backgroundColor: 'blue', padding: '20px' }}>
  <p>Customizable Content</p>
</Modal>
```

### CSS Classes Used
- `.modal-overlay`: Styles the overlay/background of the modal.
- `.modal`: Styles the modal container itself.
- `.modal-content`: Styles the content area within the modal.
- `.close-modal`: Styles the close button inside the modal.

#### Example Custom Styling

```css
.modal-overlay {
  background: rgba(0, 0, 0, 0.5);
  display: flex;
  justify-content: center;
  align-items: center;
}

.modal {
  background: white;
  padding: 20px;
  border-radius: 8px;
  max-width: 500px;
  width: 100%;
}

.close-modal {
  background: none;
  border: none;
  font-size: 1.2rem;
  position: absolute;
  top: 10px;
  right: 10px;
  cursor: pointer;
}
```
## Authors

- [@ElMoucheh](https://github.com/ElMoucheh)