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