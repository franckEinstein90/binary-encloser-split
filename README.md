```
const result = binaryEncloserSplit("no parenthesis here");
expect(result).to.deep.equal(["no parenthesis here"]);

const result = binaryEncloserSplit("this (has) (parenthesis)");
expect(result).to.deep.equal(["this", "has", "parenthesis"]);

const result = binaryEncloserSplit("this (has) (parenthesis (with) (nested) parenthesis)");
expect(result).to.deep.equal(["this", "has", "parenthesis (with) (nested) parenthesis"]);

const result = binaryEncloserSplit("( this sentence (has)) (two blocks, (each) with (nested) parenthesis)");
expect(result).to.deep.equal(["this sentence (has)", "two blocks, (each) with (nested) parenthesis"]);

```