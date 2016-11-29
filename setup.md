### Setup 

To add Scratch in your `npm` dependencies list, run:

    npm install @scratch-css/scratch --save

---
    
You need to import it in your CSS file afterwards:
  
    @import '@scratch-css/scratch';
    
Or import from `node_modules` path:

    @import './node_modules/@scratch-css/scratch/index.css';

---

Try to add this snippet in your CSS just to check if it works:

    body { background-color: var(--success) !important; }
    
Background must be green, [is not it](https://github.com/scratch-css/scratch/issues)?