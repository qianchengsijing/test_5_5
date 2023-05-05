# test_5_5
#include <stdio.h>
#include <stdlib.h>
//二叉树的顺序存储
#define MaxSize 100
typedef TreeNode{
	Elemtype value;
	bool Empty;
};
void testTree()
{
	TreeNode t[MaxSize];
	//初始化
	for(int i=0;i<MaxSize;i++)
    {
	    t[i].Empty = true;
	}
}
//链式存储
typedef Elemtype{
	int value;
};
typedef struct BiTNode{
	Elemtype data;
	struct BiTNode *lchild,*rchild;
}BiTNode,*BiTree;
typedef struct BiTNode{
	Elemtype data;
	struct BiTNode *lchild,*rchild;
	struct BiTNode *parent;//添加父结点指针
}BiTNode,*BiTree;
void testTree()
{
	BiTree root = NULL;//定义一个二叉树
	//插入根结点
	root = (BiTree)malloc(sizeof(BiTNode));
	root->data = {1};
	root->lchild = NULL;
	root->rchild = NULL;
	//插入一个新结点
	BiTNode *p = (BiTNode*)malloc(sizeof(BiTNode));
	p->data = {2};
	p->lchild = NULL;
	p->rchild = NULL;
	root->lchild = p;//作为根节点的左孩子
}
