import java.util.LinkedList;
import java.util.Queue;
import java.util.Stack;

public class ReverseQueue {
    public static void main(String[] args) {
        Queue<Integer> queue = new LinkedList<>();
        queue.add(10);
        queue.add(20);
        queue.add(30);
        queue.add(40);

        reverse(queue);

        //  طباعة الطابور بعد العكس
        while (!queue.isEmpty()) {
            System.out.print(queue.poll() + " ");
        }
    }

    public static void reverse(Queue<Integer> queue) {
        Stack<Integer> stack = new Stack<>();

        //  نقل العناصر إلى الستاك لعكس الترتيب
        while (!queue.isEmpty()) {
            stack.push(queue.poll());
        }

        //  إعادة العناصر للطابور بالترتيب المعكوس
        while (!stack.isEmpty()) {
            queue.add(stack.pop());
        }
    }
}
