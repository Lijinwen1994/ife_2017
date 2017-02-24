#自定义的css3自选框样式，<br/>
* 每个组件都装在<label>标签中，input用display:none隐藏，这样隐藏后不占位置。 用一个div写自定义样式，位置必须跟在input之后，从而可以用相邻兄弟选择器 “+” 选中。
选择器用法的重点如  `.icheck-radio > input:checked + .icheck-media`
* 可以利用伪类（after before）来样式，从而减少额外的标签，简化结构。<br/>
[点击查看demo效果](https://lijinwen1994.github.io/ife_2017/自定义选框样式/)
