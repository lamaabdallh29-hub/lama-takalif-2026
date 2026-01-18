class ListNode {
    int val;
    ListNode next;
    ListNode(int val) { this.val = val; }
}

public class RotateLinkedList {
    public ListNode rotateRight(ListNode head, int k) {
        if (head == null || k == 0) return head;

        //  حساب الطول
        int length = 1;
        ListNode tail = head;
        while (tail.next != null) {
            tail = tail.next;
            length++;
        }

        k = k % length; //  تقليل k إذا كانت أكبر من الطول
        if (k == 0) return head;

        //  ربط النهاية بالبداية لتشكيل دائرة
        tail.next = head;

        //  إيجاد نقطة القطع
        for (int i = 0; i < length - k; i++) {
            tail = tail.next;
        }

        ListNode newHead = tail.next;
        tail.next = null; //  قطع الدائرة

        return newHead;
    }
}
