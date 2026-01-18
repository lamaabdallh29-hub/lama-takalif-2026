public void deleteAtPosition(CircularNode head, int pos) {
    if (head == null || pos < 0) return;

    CircularNode current = head;
    if (pos == 0) {
        //  حذف الرأس
        while (current.next != head) current = current.next;
        current.next = head.next;
        head = head.next;
        return;
    }

    for (int i = 0; i < pos - 1; i++) {
        current = current.next;
        if (current.next == head) return; //  تجاوز الطول
    }

    current.next = current.next.next;
}
