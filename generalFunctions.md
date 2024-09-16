Binary Search

lb Binary Search

ub Binary Search

# Trie

```
public List<String> searchKeys(TrieNode node, String text, int index){
    List<String> res = new ArrayList<>();
    int count = 0;
    for(int i=index;i<text.length();i++){
        if(node.endOfWord)  res.add(index+"-"+(i-1));
        if(node.child[text.charAt(i)-'a']!=null){
            node = node.child[text.charAt(i)-'a'];
        } else {
            return res;
        }
    }
    if(node.endOfWord)  res.add(index+"-"+(text.length()-1));
    return res;
}

public void insertKeys(TrieNode node, String key){
    for(char c:key.toCharArray()){
        if (node.child[c - 'a'] == null) {
            TrieNode newNode = new TrieNode();
            node.child[c - 'a'] = newNode;
        }
        node = node.child[c - 'a'];
    }
    node.endOfWord = true;
}

class TrieNode{
    TrieNode[] child;
    boolean endOfWord;
    TrieNode(){
        child = new TrieNode[26];
        endOfWord = false;
    }
}

```
