Goal of this repo is to evaluate options of CSS-in-JS with ShadowDom

## styled-jsx
```javascript

const { className, styles } = css.resolve`
  color: green;
`;

const StylesElem = (styles as unknown) as React.Component;

const StyleTag: React.FC = () => (
  <style>{StylesElem.props.children}</style>
);
```
