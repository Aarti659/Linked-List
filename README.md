// Linked list implementation in C++

#include <bits/stdc++.h>

#include <iostream.h>

using namespace std;


class Node {
   public:
  int val;
  Node* nex;
};

int main() {
  Node* head;
  Node* one = NULL;
  Node* two = NULL;
  Node* three = NULL;


  one = new Node();
  two = new Node();
  three = new Node();

  
  one->val = 1;
  two->val = 2;
  three->val = 3;

  
  one->nex = two;
  two->nex = three;
  three->nex = NULL;

  
  head = one;
  while (head != NULL) {
    cout << head->val;
    head = head->nex;
    return 0;
  }
}





