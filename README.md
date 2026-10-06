# git_test

Git `cherry-pick` 연습용 저장소입니다.

## 브랜치 구조

```
c1 ─ c2 ─┬─ m1 ─ m2 ─ m3 ─ f1'   (main)
         └─ f1 ─ f2              (fight)
```

- `main`: m1 ~ m3에서 `Hello.txt` Section 1에 인사말 추가
- `fight`: f1에서 Section 2에 `Bye world!` 추가, f2에서 Section 1에 `Fight` 추가

## 연습 내용

1. `fight`의 f1을 `main`으로 cherry-pick (충돌 없음)
2. `fight`의 f2를 `main`으로 cherry-pick (Section 1에서 충돌 발생 → 직접 해결)

```bash
git cherry-pick <커밋>
git cherry-pick --continue   # 충돌 해결 후
git cherry-pick --abort      # 취소
```

## License

[MIT](LICENSE)
