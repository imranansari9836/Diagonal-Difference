     public static int diagonalDifference(List<List<Integer>> arr) {
        int a = 0, b = 0;
        for(int i = 0; i < arr.size(); i++){
            for(int j = 0; j < arr.size(); j++){
                if(i == j){
                    a += arr.get(i).get(j);
                }
                if((i + j) == (arr.size() - 1)){
                    b += arr.get(i).get(j);
                }
            }
        }
        return Math.abs(a-b);
    }

}
