Metodo 1:
Babel configuration

.babelrc
{
  "presets": ["@babel/preset-env", "@babel/preset-react"],
  "plugins": ["@babel/plugin-proposal-class-properties"]
}

Metodo 2:
Agregando constructor en las clases

constructor() {
    super();
    this.state = {
      seo_title: ""
    };
    this.handleChange = this.handleChange.bind(this);
}

Metodo 3:
Stateless funciotnal components (no clases)

Usando hooks y no states


--------------------

Referencias:
https://github.com/desaijay315/react-webpack-boilerplate
https://www.valentinog.com/blog/babel/
https://blog.usejournal.com/setting-up-react-webpack-4-babel-7-from-scratch-2019-b771dca2f637