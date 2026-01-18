import java.util.Stack;

public class SortStack {
    public static void main(String[] args) {
        Stack<Integer> original = new Stack<>();
        original.push(34);
        original.push(3);
        original.push(31);
        original.push(98);
        original.push(92);
        original.push(23);

        Stack<Integer> sorted = sortStack(original);

        //  طباعة الستاك المرتب
        while (!sorted.isEmpty()) {
            System.out.print(sorted.pop() + " ");
        }
    }

    public static Stack<Integer> sortStack(Stack<Integer> input) {
        Stack<Integer> tempStack = new Stack<>();

        while (!input.isEmpty()) {
            int temp = input.pop();

            //  نقل العناصر الأكبر مؤقتًا للستاك الأصلي
            while (!tempStack.isEmpty() && tempStack.peek() > temp) {
                input.push(tempStack.pop());
            }

            tempStack.push(temp); //  إدراج العنصر في مكانه الصحيح
        }

        return tempStack;
    }
}
