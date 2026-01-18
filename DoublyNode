class DoublyNode {
    int val;
    DoublyNode prev, next;
    DoublyNode(int val) { this.val = val; }
}

public void removeDuplicates(DoublyNode head) {
    HashSet<Integer> seen = new HashSet<>();
    DoublyNode current = head;

    while (current != null) {
        if (seen.contains(current.val)) {
            //  إزالة العنصر
            if (current.prev != null) current.prev.next = current.next;
            if (current.next != null) current.next.prev = current.prev;
        } else {
            seen.add(current.val);
        }
        current = current.next;
    }
}
