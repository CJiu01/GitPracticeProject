# Git Practice Project

## How to write Commit Message && Pull Request Message

커밋 메시지나 PR 타이틀을 작성할 때 아래의 예시에 있는 것과 같이 \
대괄호를 열고 태그를 작성해주세요 😆 😆

1. 파일 추가 : Add
2. 버그 수정 : Fix
3. 리팩터링 : Refactoring
4. 주석 추가 : Comment
5. 파일 삭제 : Remove
6. 기능 추가 : Feat
7. 문서 수정 : Docs

> Ex) [Feat] Len 함수 기능 완성

## Participants

원하는 정보 입력하시면 됩니다 😍 😍

|  Name  |          Email           |
| :----: | :----------------------: |
| 최지웅 | jwchoi179@soongsil.ac.kr |
| 김현수 |  rover0811@hotmail.com   |
| 김지은 |   wldmsk0918@gmail.com   |
| 김선환 | rlatjsghks4647@naver.com |
|  유진  | jini1514@soongsil.ac.kr  |
| 이정훈 |  dominanthat@gmail.com   |
| 최지우 |  jiwoo020801@gmail.com   |
| 홍준혁 |  junhyeok2166@daum.net   |

## Purpose

이 레포지토리는 Pull Request를 포함한 \
`Git`을 사용하여 협업을 연습하는 시간을 가져봅니다.

## Parts

### Account Class

```C++
class Account {
private:
  int accountID;
  int balance;
  char *cusName;

public:
  // 김현수 담당
  Account(int ID, int money, char *name);
  Account(const Account &ref);

  int GetAccID() const;
  // 최지우 담당
  void Deposit(int money);

  // 김지은 담당
  int Withdraw(int money);

  // 유진 담당
  void ShowAccInfo() const;
  ~Account();
};
```

### Account Handler Class

```C++
class AccountHandler {
private:
  Account *accArr[100];
  int accNum;

public:
  AccountHandler();
  void ShowMenu(void) const;

  // 이정훈 담당
  void MakeAccount(void);

  // 홍준혁 담당
  void DepositMoney(void);

  // 김선환 담당
  void WithdrawMoney(void);

  // 최지우 담당
  void ShowAllAccInfo(void) const;
  ~AccountHandler();
};
```
