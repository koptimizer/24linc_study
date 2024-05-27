# Modeling
- gurobi와 gurobipy에 대해서 학습하고 아래의 문제를 해결하기
- <b>하나의 .ipynb파일(쥬피터 랩 확장자)로 답안 파일을 만들고, 각 문제를 블록 단위로 구별하여 코딩할 것!.</b>
- <b>코드에 대한 주석 작성 필수</b>
</br>

### Modeling with Gurobi
1. <b>하기 4종류의 Location problem을 이해하고, 차이점을 정리하라.</b>
   1. P-median
   2. P-center
   3. Set covering
   4. Maximal covering
   5. Fixed-charge location problem
   
2. <b>Multi-Depot Capaciated Vehicle Routing Problem을 위한 problem generator 및 mathmatical model을 gurobi로 구현하라.</b> 
   1. Node는 depot, customer로 구성되고, 요소 각각 여러개가 배치될 수 있다.
   2. Vehicle은 depot에서 출발해서 여러명의 customer에게 물건을 배송한뒤 다시 자신이 출발했던 depot으로 돌아와야 한다.
   3. 각 depot에서 사용가능한 vehicle 무제한이나, vehicle을 사용할 떄 고정비용 $a$ 가 발생한다.
   4. 각 vehicle은 동일한 capacity $c$ 를 가지며, 이동거리에 비례해서 비용이 발생한다.
   5. 각 customer의 demand는 1이며, 단 한개의 depot과 vehicle만 할당받는다.
   7. 목표는 비용의 최소화이다.
   8. Problem Generator에서는 depot은 2-5, customer node는 10-100까지 설정이 가능해야하며, 문제에 포함되는 각 파라미터를 조정할 수 있어야 한다.
   9. LP 파일을 뽑아서 이를 해석할 수 있어야 한다.
  
2. <b>Multi-Depot Capaciated Vehicle Routing Problem을 위한 Genetic Algorithm(GA)을 구현하라.</b> 
   1. Solution representation에 대한 제약은 없다.
   2. Crossover, mutation operator는 feasible-guaranteed로 구현한다.
   3. Tournament selection을 사용하고, selection pressure를 조정가능할 수 있도록 한다.
   4. Large size problem instance에 대해서 구현한 mathmatical model과 GA를 비교한다.  
    
