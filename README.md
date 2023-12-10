# react-query
cheerio like functions for react element query

```
import React from "react"
import ReactQuery from "react-query"
const el=(
    <div>
        <span>hello</span>
    </div>
)

const $=new ReactQuery(el)
const span=$.findFirst('span').get(0)

const updatedEl=$.replace(span, <i>hello</i>, {["id":"ui"]}).root
/**
* updatedEl is 
    <div>
        <i id="ui">hello</i>
    </div>
*/

```