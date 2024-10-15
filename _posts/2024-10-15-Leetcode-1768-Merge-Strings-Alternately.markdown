
postname_리트코드75로_코테준비_재시작_미리시작
link_https://leetcode.com/problems/merge-strings-alternately/description/
code_asbelow
```code=js
/**
 * @param {string} word1
 * @param {string} word2
 * @return {string}
 */
const max = (a, b) => a > b ? a : b

var mergeAlternately = function(word1, word2) {
    let merged = ""
    const lengthWord1 = word1.length
    const lengthWord2 = word2.length
    for(let i = 0; i < max(lengthWord1, lengthWord2); i++) {
        merged += word1[i] || ""
        merged += word2[i] || ""
    }
    return merged
};
```
