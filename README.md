# java_4day_condition
조건문



과제1. 입사시험문제/실무문제 나눠서 정리. 면접때 대비


과제2. 연산자

1) 대입연산자
2) 연결연산자
3) 사칙연산자
4) 증감연산자
5) 비교연산자
6) 논리연산자
7) 삼항연산자

//# 중요 #ㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡ		
//국어점수 95, 영어점수 88, 수학 77

			int kor = 90;
			int eng = 84;
			int mat = 90;
			
//총점
      
			int tot = kor + eng + mat;
			
//평균***************시팔.. 자바..

			double avg = (double)tot/3;
      
// cast 연산자.
// 왜 double로 타입 캐스팅을 해야하는가!?
//
			
			System.out.println(avg);
      
//# 중요 #ㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡ
			
			String hakjum = ""; 
//(""길이가 없는 문자 데이터.)(" "공백도 데이터다.)
//나중에 갱신하자는 의미
					
				if (avg >= 90 && avg <= 100 ) {					
					hakjum = "a";					
				}

				else if (80 <= avg && avg < 90 ) {    	
					hakjum = "b";    	
				}
	
				else if (70 <= avg && avg < 80 ) {    	
					hakjum = "c";    	
				}

				else if (60 <= avg && avg < 70 ) {	
					hakjum = "d";	
				}  
				else if (0 <= avg && avg < 60 ) {	
					hakjum = "f";	
				} else {
					hakjum = "학점 정보 없음";
				}
        
				System.out.println(hakjum);	
//초기화 안됐는데 왜
//프로그램 입장에서 100 넘어가면 조건문에 속해지지 않는데
//데이터가 없는데 그걸 찍으라고?				
//지역변수는 일단 아무런 값이라도 집어넣고 시작해라. 
//그래야 뒤탈이 없다.
				
//조건문에 무조건 걸리게 하면 
//조건이 겹치면 if/else if의 순서를 조심해야한다.
				
				
//ㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡ
				
				
				if (avg >= 90 && avg <= 100 ) {					
					hakjum = "a";					
				}

				else if (60 <= avg ) {	
					hakjum = "d";	
				}
				
				else if (80 <= avg) {    	
					hakjum = "b";    	
				}
	
				else if (70 <= avg ) {    	
					hakjum = "c";    	
				}

  
				else if (0 <= avg && avg < 60 ) {	
					hakjum = "f";	
				} else {
					hakjum = "학점 정보 없음";
				}
        
				System.out.println(hakjum);	
	
/*ㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡ
		평균이 80이 넘으면 "합격"을 출력하고
		평균이 80 미만이면 "불합격"을 출력하세요					
ㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡ*/
				
				
			int sbj1 = 80;
			int sbj2 = 91;
			int sbj3 = 90;
			int sbj4 = 95;
			int sbj5 = 90;
			
			int total = sbj1 + sbj2 + sbj3 + sbj4 + sbj5;
			double avarage = (double)total/5;
			
			
			String result = "";
			
			if (avarage > 80) {
					result = "합격";
			} else {
					result = "불합격";
			}

//합격불합격 변수 하나 만들자.
//추후에 또 사용할 수 있기 때문에 
// result라는 변수를 하나 만들어서 집어 넣자			
			
//ㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡ
//삼항연산자

			result = ( avarage > 80) ? "합격" : "불합격";
      
//ㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡ
			
			System.out.println(result);	
      
		
//ㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡ
// 아래 조건을 만족하면 "합격" 만족하지못하면 "불합격"
// 조건은 평균 60이상, 각 과목이 40이상 
// 국영수
//ㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡ
			
			int kor1 = 10;
			int mat1 = 95;
			int eng1 = 80;
			
			int tot1 = kor1 + mat1 + eng1;
			
			double avg1 = (double)tot1/3;
			
			String result1 = "";
			
			if (avg1 < 60 || mat1 < 40 || eng1 < 40 || kor1 < 40) {
	
				result1 = "불합격";
	
			}else {
				result1 = "합격";
			}
			
			
			System.out.println("국어 점수 = " + kor1);
			System.out.println("수학 점수 = " + mat1);
			System.out.println("영어 점수 = " + eng1);
			System.out.println("과목 평균 = " + avg1);
			System.out.println("시험 결과 = " + result1);
	}
	

}
