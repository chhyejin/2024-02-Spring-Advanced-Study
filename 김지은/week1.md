## 내용정리

-링크 : https://dsc-sookmyung.tistory.com/629

## 느낀점
: 관심사의 분리가 전혀 이루어지지 않은 초난감 DAO에서부터 컨테이너의 도입까지 단계적으로 발전시키는 과정을 따라가볼 수 있어서 스프링의 근본적인 목표를 다시 생각해보게 돼서 좋았습니다.
특히 인스턴스 변수 사용에 주의해야 하는 점을 프로젝트 할 때 잊고 있었는데, 다시 한 번 생각해볼 기회가 됐습니다.

## 질문정리
- 의존성 주입(DI) 방법 세 가지 설명하기
  
  1. 수정자메소드(setter)
   : set으로 시작하며 + 한 개의 파라미터만 갖는, 내부의 애트리뷰트 값 변경 목적의 수정자 메소드를 통해 값 주인이 가능하다. 파라미터로 전달된 값을 내부의 인스턴스 변수에 저장한다
  2. 필드주입(일반메소드)
    : 여러 개의 파라미터를 가질 수 있어 여러 필드의 초기화 메소드를 만들 수 있다
  3. 생성자메소드
    : 순환참조를 방지하며 + 런타임의 불변성을 보장할 수 있다(final) + 테스트코드 작성에 유리하다