# wp-idg-ufr__block-components

> Componentes utilizados nos blocos do tema WP da Universidade Federal de Rondonópolis <br />
> !Importante -> Depende de github.com/juniorjmm/wp-idg-ufr__block_dependencies, que deve estar instalado como um plugin no WP

[![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)

## Instalação

```bash
npm install https://github.com/juniorjmm/wp-idg-ufr__block-components.git
```

## Uso

### Importe e use
```jsx
import React, { Component } from 'react'

import { UFRComponente } from 'wp-idg-ufr__block-components'

class Example extends Component {
  render() {
    return <UFRComponente prop1={var1} />
  }
}
```

### Componente ```<UFRBlockHeader /> ```
Atributos:
  - title: string // Para exibição no título
  - subtitle: string // Para exibição no subtítulo

### Componente ```<GaleryBtn /> ```
Atributos:
- text: string // Para exibição no título
- icon: string // Para exibição no subtítulo
- allowedTypes: string[] // Tipos permitidos para upload
- setter: function // Função 'setAttributes' provida nos parâmetros do método 'edit' no ambiente @wodpress/create-block
- attr: string // Atributo para ser alterado com o setter, listado em block.json na seção 'attributes'

### Componente ```<IconPicker /> ```
Atributos:
- setter: function // Função 'setAttributes' provida nos parâmetros do método 'edit' no ambiente @wodpress/create-block

### Componente ```<Input /> ```
Atributos:
- label: string // atributo label nativo do input
- type: string // atributo type nativo do input, defaults to 'text'
- value: string // atributo value nativo do input
- className: string // attributo className nativo do React
- setter: function // Função 'setAttributes' provida nos parâmetros do método 'edit' no ambiente @wodpress/create-block
- attr: string // Atributo para ser alterado com o setter, listado em block.json na seção 'attributes'
-
### Componente ```<Select /> ```
Atributos:
- label: string // atributo label nativo do input
- options: { label: string, value: string | boolean | number }[] // Array de opções para o select
- value: string | boolean | number // atributo value nativo do input
- setter: function // Função 'setAttributes' provida nos parâmetros do método 'edit' no ambiente @wodpress/create-block
- attr: string // Atributo para ser alterado com o setter, listado em block.json na seção 'attributes'
