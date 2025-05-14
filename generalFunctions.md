Binary Search
```java
/**
 * Binary‑search helpers for **sorted** (ascending) int arrays.
 *
 * All methods run in O(log n) time and O(1) space.
 */
public final class BinSearch {

    private BinSearch() {}            // utility class ⇒ no instances

    /** Classic binary search: returns index of target or ‑1 if not present. */
    public static int binarySearch(int[] a, int target) {
        int lo = 0, hi = a.length - 1;
        while (lo <= hi) {
            int mid = lo + (hi - lo) / 2;
            if (a[mid] == target) return mid;
            if (a[mid] < target)   lo = mid + 1;
            else                   hi = mid - 1;
        }
        return -1;
    }

    /**
     * Lower bound: first index whose value is ≥ target.
     * If every element is < target, returns a.length (i.e., “insert at end”).
     */
    public static int lowerBound(int[] a, int target) {
        int lo = 0, hi = a.length;          // hi is exclusive
        while (lo < hi) {
            int mid = lo + (hi - lo) / 2;
            if (a[mid] < target) lo = mid + 1;
            else                 hi = mid;   // keep mid (it’s ≥ target)
        }
        return lo;
    }

    /**
     * Upper bound: first index whose value is > target.
     * If every element is ≤ target, returns a.length.
     */
    public static int upperBound(int[] a, int target) {
        int lo = 0, hi = a.length;          // hi is exclusive
        while (lo < hi) {
            int mid = lo + (hi - lo) / 2;
            if (a[mid] <= target) lo = mid + 1;
            else                  hi = mid; // keep mid (it’s > target)
        }
        return lo;
    }

    /* ── tiny demo ─────────────────────────────────────────────── */
    public static void main(String[] args) {
        int[] nums = {1, 3, 3, 5, 7, 7, 7, 9};

        System.out.println(binarySearch(nums, 5));   // 3
        System.out.println(lowerBound(nums, 7));     // 4
        System.out.println(upperBound(nums, 7));     // 7
        System.out.println(lowerBound(nums, 4));     // 3  (insert pos)
        System.out.println(upperBound(nums, 10));    // 8  (end of array)
    }
}


```

# Trie

```haa 
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
