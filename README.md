# Data-Structures
BECS 21223 

class Stack1 {
    private int max;
    private int top;
    private char[] array1;

    Stack1(int max) {
        this.max = max;
        array1 = new char[max];
        top = -1;
    }
    public boolean isStackFull() {
        return top == max - 1;
    }
    public boolean isStackEmpty() {
        return top==-1;
    }
    public char pop() {
        if (isStackEmpty()) {
            System.out.println("Stack is empty");
        }
            return array1[top--];
    }
    public void push(char char1){
        if(isStackFull()){
            System.out.println("Stack is full");
        }
        else {
            System.out.println("Insert "+char1);
            array1[++top]=char1;
        }
    }
    public void reverse(){
        for(int i=0;i<max;i++){
            System.out.print(pop());
        }
    }
}
class One{
    public static void main(String[] args){
        char[] a1={'a','b','c','d','e'};
        int size =a1.length;
        Stack1 s1=new Stack1(size);
        for(int x=0;x<size;x++) {
            s1.push(a1[x]);
        }
        s1.reverse();
    }
}
public void reverse(){
        for(int i=0;i<max;i++){
        System.out.println(array1.);
         }
    }
