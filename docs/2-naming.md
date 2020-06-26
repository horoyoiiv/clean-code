
2.의미 있는 이름
======================


2.1. 의도를 분명히 밝혀라
---------------------

변수, 함수, 클래스 명은 다음의 질문에 답할 수 있어야 한다.  
> 변수, 함수, 클래스의 존재 이유는? 수행 기능은? 사용 방법은?  
주석이 필요로 한다면 의도를 분명히 드러내지 못했다는 말이다.
 
```
[Bad]
int d;

[Good]
int elapsedTimeInDays;
int daysSinceCreation;
int daysSinceModification;
int fileAgeInDays;
```
<br/>

2.2. 그릇된 정보를 피하라
----------------------
휼륭해 보이는 **약어**(Abbreviation or Acronym)일지라도 독자에게 그릇된 정보를 제공할 수 있다.  
여러 계정을 그룹화할 때, 실제 List가 아니면 accountList라고 명명하지 않는다.  
> 개발자에게 List란 특수한 의미를 가지기 때문이다. 
 
```
[Bad]
accountList

[Good]
accountGroup
bunchOfAccounts
Accounts
```

<br/>

2.3. 의미 있게 구분하라
---------------------- 
Product 클래스가 있을 때, ProductInfo 혹은 ProductData 클래스가 등장한다면 **개념이 구분되지 않는 것이다.**  
```
// 이 프로젝트에 참여한 프로그래머는 어느 함수를 호출할지 어떻게 알까?

getActiveAccount();
getActiveAccounts();
getActiveAccountInfo();
```

<br/>

2.4. 발음하기 쉽고, 검색하기 쉬운 이름을 사용하라
-----------------------------------------

```
class DtaRcrd102 {
  private Date genymdhms;
  private Date modymdhms;
  private final String pszqint = "102";
}

class Customer {
  private Date generationTimestamp;
  private Date modificationTimestamp;
  private final String recordId = "102";
}
```

<br/>

## 💍 명료함이 최고다.  

<br/>

2.5. 클래스 이름과 메서드 이름
---------------------------
클래스 이름과 객체 이름은 **명사**나 **명사구**가 적합하다.  
> Manager, Processor, Data, Info 등과 같은 단어는 피하고, 동사는 사용하지 않는다.  
Customer, WikiPage, Account, AddressParser 등이 좋은 예이다.  

메서드 이름은 **동사**나 **동사구**가 적합하다.  
> postPayment, deletePage, save 등이 좋은 예이다. 
 
생성자를 중복정의(Overload)할 때는 **정적 팩토리 메서드**를 사용한다.  
> 메서드는 인수를 설명하는 이름으로 사용된다. 



<br/>

2.6. 한 개념에 한 단어만 사용하라
---------------------- 
가져온다는 개념의 메서드를 get, fetch, retrieve 등 제각각으로 부르면 혼란스럽다.  
> 기존의 add 메서드는 모두 두 값을 더하여 그 결과를 반환하는데, 새로 작성된 메서드에서는 집합에 원소를 추가할 때 이를 add 메서드로 명명해도 괜찮은가? 새 메서드는 기존의 add 메서드와 문맥이 다르기에, insert, append가 적합하다. 

<br/>

2.7. 
 




