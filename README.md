# jblock
a high-level block-based visual programming language


```js
import React from 'react';
import { Control, Input } from '@/comps';

const times = (props) => {
  const { value, ...others } = props;
  return (
    <Control text="重复执行{?}次" icon="logo" {...others}>
      <Input inputType="number" value={value} />
    </Control>
  );
};

times.defaultProps = {
  type: 'times',
  area: 1, // important
  value: 3,
};

const compiler = async (block, target) => {
  //
};

export { times, compiler };
```
