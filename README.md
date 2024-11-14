
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

- `isOpen` (`boolean`,required): Controls whether the modal is visible.
- `onClose ` (`function`,required): Controls whether the modal is visible.
- `children  ` (`ReactNode`,required): Controls whether the modal is visible.


## Authors

- [@ElMoucheh](https://github.com/ElMoucheh)

