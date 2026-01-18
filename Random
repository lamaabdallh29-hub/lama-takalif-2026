import java.util.Random;

public class RemoveRandomElement {
    public static void main(String[] args) {
        int[] original = {10, 20, 30, 40, 50};
        Random rand = new Random();
        int indexToRemove = rand.nextInt(original.length); //  تأكد أن الفهرس داخل حدود المصفوفة

        int[] result = new int[original.length - 1];
        for (int i = 0, j = 0; i < original.length; i++) {
            if (i != indexToRemove) {
                result[j++] = original[i];
            }
        }

        //  طباعة النتيجة
        for (int num : result) {
            System.out.print(num + " ");
        }
    }
}
