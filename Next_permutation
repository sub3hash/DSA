class Solution{
    static List<Integer> nextPermutation(int N, int arr[]){
        List<Integer> arlist=new ArrayList<Integer>();
        int index=-1;
        for(int i=N-2;i>=0;i--)
        {
            if(arr[i]<arr[i+1])
            {
                index=i;
                break;
            }
        }
        for(int k=0;k<N;k++)
        {
            arlist.add(arr[k]);
        }
        if(index==-1)
        {
            Collections.reverse(arlist);
            return arlist;
        }
        for(int j=N-1;j>index;j--)
        {
            if(arr[j]>arr[index])
            {
                int temp=arlist.get(j);
                arlist.set(j,arr[index]);
                arlist.set(index,temp);
                break;
            }
        }
        List<Integer> sublist=arlist.subList(index+1,N);
        Collections.reverse(sublist);
        return arlist;
    }
}
