# InvaderSurvive_Final

시작 : 2025.04 <br/>
[ 상태 관리 ]<br/>
1. PlayerCore에서의 Locomotion, Combat 관리 <br/>
2. Locomotion과 Combat 상태들 FSM + Strategy패턴으로 관리  <br/>
3. MainState(주력 단일 상태) + Flags(복수개)를 활용한 SubState 적용  <br/>

PlayerCore <br/>
├── 공통 <br/>
│   ├── Rigidbody 관리 (PlayerPhysicsUtility) <br/>
│   ├── 입력 매니저, 애니메이션 매니저 참조 <br/>
│   └── 공통 기능 (Collider 스위치 등) <br/>
├── Locomotion <br/>
│   ├── PlayerLocomotion 모듈 초기화 <br/>
│   ├── 속도, 회전 값 세팅 <br/>
│   └── 이동 관련 Update/FixedUpdate 호출 <br/>
└── Combat <br/>
    ├── PlayerCombat 모듈 초기화 (예정) <br/>
    ├── 공격, 피격 처리 <br/>
    └── 전투 관련 Update/FixedUpdate 호출 <br/>
