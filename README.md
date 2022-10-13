# Print-Single-LinkedList
public class SingleLinkedList {
    public void Print(Node head)

    {
        if(head==null)
        {
            return;
        }
        Node current=head;
        while(current!=null)
        {
            System.out.println(current.data);
//node=node.next;
current=current.next;
        }
       // System.out.println(current);
    }


    public static class Node{
        int data;
        Node next;
        Node(int data)
        {
           this.data=data;

        }
    }
    public static void main(String[] args)
    {

        SingleLinkedList obj=new SingleLinkedList();
        Node head=new Node(2);
        Node one=new Node(3);
        Node two=new Node(4);
        Node tree=new Node(5);
        head.next=one;
        one.next=two;
        two.next=tree;
        obj.Print(head);
    }
    
}
