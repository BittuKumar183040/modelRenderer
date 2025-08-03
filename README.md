
# Result Rendering

This is a repository which is mojorly resposible for render the **result file of extension** *.vtk which is of type _unstructured data_.

## Technologies Used

- [React](https://beta.reactjs.org/)
- [Tailwind CSS](https://tailwindcss.com/)
- [Regular Expression](https://regexr.com/)
- [GLSL](https://developer.mozilla.org/en-US/docs/web/api/webgl_api/tutorial/getting_started_with_webgl)
- [React Three Fiber](https://docs.pmnd.rs/react-three-fiber/getting-started/introduction)

## Coding Standards (Front-End)

- Use functional components; avoid class-based components.
- Keep components small, reusable, and loosely coupled.
- Separate logic and UI components into different folders.

  ```jsx, js
  - src
    |-- components
    |   |-- Graph.js        [Side colormap which shows color, max and min displacemnt and value lie between them]
    |   |-- FileUpload.js
    |   |-- Heatmap.js
    |   |-- Inner.js        [Responsible for rendering and compering displacemnts]
    |   |-- Loading.jsx
    |-- App.js
    |-- VtkRendering.jsx    [This file contains Canvas and most of the rendering Functions]
  ```

  - **components:** Reusable components.
  
- Report UX bugs promptly.
- Define routing and state management standards during project development.
- Test app performance using tools like Lighthouse.

### Docker Instructions
- Build the image 
  <code>docker build -t vtkrenderer .</code><br>
- Run the image
  <code>docker run -d -p 3000:3000 vtkrenderer</code>

