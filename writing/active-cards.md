# Active Cards — Q3 글쓰기 능동화 카드

> chunk·함정·정형표현·연결사를 **한 파일**에서 4-tier + SRS로 관리하는 통합 카드 시스템.
> **`/write`가 자동 관리한다** — 작문 첨삭 중 chunk 추출·Tier 분류·복습 스케줄을 Claude가 처리.
> 사용자 부담은 "작문 + OK 한 번". (drill처럼 따로 호출하면 안 쓰니까 /write에 통합)

---

## 시스템 정의

### 4-tier (부담 조절)

| Tier | 의미 | 처리 | 분량 |
|------|------|------|------|
| **T1** | 오늘의 적극 학습 | 의식적 반복 + 다음날 워밍업 출제 | 1\~2개 |
| **T2** | 단기 복습 | 워밍업 회전 출제 | 5\~10개 |
| **T3** | 간격 반복 (정착) | SRS 자동 스케줄 | 제한 없음 |
| **T4** | 참조 보관 | 카드만 보관, 능동 학습 X | 제한 없음 |

> 핵심 원칙: **모든 오류 카드화 ≠ 모든 오류 의식 학습.** 매일 N개 나와도 T1으로 올릴 건 **1\~2개만** 선택. 나머지는 카드만 누적.

### 카테고리

| 코드 | 의미 | 예 |
|------|------|-----|
| **chunk** | 써야 할 collocation | en terrasse, prendre une décision |
| **cliché** | 한국어 화자 함정 (회피 패턴) | à la terrasse → en terrasse |
| **formule** | 글의 뼈대 정형표현 | Pour ma part, je pense que… |
| **connecteur** | 연결사 | donc, néanmoins, par ailleurs |

### register (사용역)

| 코드 | 의미 | 사용 분기 |
|------|------|----------|
| **W** | 문어 (écrit) | Q3 글쓰기 |
| **O** | 구어 (oral) | Q4 말하기 |
| **S** | 공유 (both) | Q3 + Q4 |

> Q3 글쓰기는 **W + S** 카드를 사용 (O는 Q4 말하기 분기에서 활성화).

### SRS 간격

1일 → 3일 → 7일 → 14일 → 30일 → 숙달(T4 인지)

### 카드 컬럼

`카테고리 | reg | 표현/패턴 | 의미·용법 | 흔한 오류(있으면) | 등록일 | 다음 복습일 | 사용횟수`

### T1 우선순위 결정 (ROI)

| 우선 | 기준 |
|------|------|
| ⭐⭐⭐ T1 | 같은 세션 2회+ 등장 / 매일 쓰이는 정형 / DELF 채점표 직격 |
| ⭐⭐ T2 | 자주 쓰이나 한 번에 외우기 부담 / 시간 지나면 자연 정착 |
| ⭐ T4 | 단발성 어휘 오류 / 향후 학습으로 자동 해소 예정 |

---

## T1 — 적극 학습 중 (1\~2개)

| 카테고리 | reg | 표현/패턴 | 의미·용법 | 흔한 오류 | 등록일 | 다음 복습일 | 사용 |
|---|---|---|---|---|---|---|---|
| grammaire | W | 서사 시제: 배경·묘사·상태=반과거 / 일어난 사건=복합과거 (과거 이야기는 현재형 금지; quand+사건=PC) | "이야기를 미는 사건→PC / 멈춰 묘사→imparfait" · 수동태는 웬만하면 X | (7/19~23 실전 정확 반복; Je dormais quand le téléphone a sonné) | 2026-07-18 | 2026-07-25 | 5 |

## T2 — 단기 복습 (5\~10개)

| 카테고리 | reg | 표현/패턴 | 의미·용법 | 흔한 오류 | 등록일 | 다음 복습일 | 사용 |
|---|---|---|---|---|---|---|---|
| chunk | W | 감정 형용사 + de + 부정사 (Je suis heureux/content/fier de…) | 감정=사람 주어+être+de (de=감정의 원인·출처). 다른 주어면 que+접속법 | C'est heureux ❌ / de être → d'être | 2026-07-13 | 2026-07-18 | 3 |
| cliché | S | 회사 = l'entreprise (travailler dans / mon·notre entreprise) | bureau≠회사 / notre l'entreprise ❌ | mon bureau(회사) ❌ | 2026-07-15 | 2026-07-19 | 3 |
| cliché | S | informer qqn ≠ communiquer/annoncer qch | 사람에게 알리다 / 결정을 통보하다 | la décision soit informé ❌ → communiquée | 2026-07-16 | 2026-07-17 | 0 |
| grammaire | W | il aurait mieux valu + 부정사 | ~하는 게 나았을 것이다 | il aurait fait mieux annoncer ❌ | 2026-07-16 | 2026-07-17 | 0 |
| cliché | S | Ce qui m'a frappé/étonné (me=직접목적어, être 없음) | frapper/étonner qqn 능동 | ce qui m'a été frappé ❌ → m'a frappé | 2026-07-18 | 2026-07-19 | 0 |
| chunk | S | être en rupture de stock | 품절이다 | toujours rare (덜 자연) | 2026-07-18 | 2026-07-19 | 0 |
| cliché | S | chaque + 단수명사 ↔ chacun(단독) | 각각의 ~ (chaque magasin) | du chacun magasin ❌ | 2026-07-18 | 2026-07-19 | 0 |
| grammaire | W | 예정된 과거 = devait + 부정사 (~할 예정이었다) | 조건법(serait)·조건법과거(aurait été) 아님 — imparfait de devoir | la cérémonie serait organisé ❌ → devait avoir lieu | 2026-07-19 | 2026-07-23 | 1 |
| cliché | S | le cours(수업, 남) ≠ la cour(마당, 여) | 철자·성으로 뜻 바뀜 | la cours(수업) ❌ | 2026-07-19 | 2026-07-20 | 0 |
| cliché | S | 요일 앞 무전치사 (avoir lieu samedi / lundi prochain) | 요일엔 à/le 없이 바로 | avoir lieu à samedi ❌ | 2026-07-20 | 2026-07-21 | 0 |
| grammaire | W | 대명사 y = à + 사물/장소 | j'y pense(penser à) / je m'y entraîne(s'entraîner à) | me l'entraîner ❌ | 2026-07-20 | 2026-07-21 | 0 |
| grammaire | W | séparer A **de** B | A와 B를 분리하다 (et 아님) | séparer vie pro et vie privée ❌ | 2026-07-21 | 2026-07-22 | 0 |
| grammaire | W | se contrôler (자기 통제) | 통제하다는 대상 필요; 자기 자신=se contrôler | contrôler soi-même ❌ / ne peut pas contrôler | 2026-07-24 | 2026-07-25 | 0 |
| grammaire | W | 소유형용사는 주어에 일치 (il→son/ses, ils→leur/leurs) | 복수 주어면 leur/leurs | Ils…son rôle ❌ → leur | 2026-07-24 | 2026-07-25 | 0 |
| grammaire | W | de + le/les = du/des (축약) | de+le=du, de+les=des | de les personnes ❌ → des | 2026-07-24 | 2026-07-25 | 0 |
| grammaire | W | aider qqn à + 부정사 | ~하도록 돕다 (주어 다르면 à로 연결, pour X) | aider pour ne pas perdre ❌ → à | 2026-07-24 | 2026-07-25 | 0 |
| grammaire | W | dire que (≠ parler que) | ~라고 말하다 (parler는 que절 안 받음) | la japonaise parle que ❌ → dit que | 2026-07-25 | 2026-07-26 | 0 |
| cliché | S | étrange(이상한) ≠ étranger(외국인·외국의) | 철자로 뜻 바뀜 | les étranges ❌ → les étrangers | 2026-07-25 | 2026-07-26 | 0 |
| chunk | S | avoir du mal à + 부정사 (du 필수) | ~하기 힘들다 (avoir mal à=아프다와 구별) | avoir mal à courir ❌ | 2026-07-27 | 2026-07-28 | 0 |
| grammaire | W | comme s'il ne s'était rien passé / comme si de rien n'était | 아무 일도 없었던 것처럼 (se passer 대과거) | comme s'il n'y avait rien ❌ | 2026-07-27 | 2026-07-28 | 0 |
| chunk | S | sans s'en rendre compte (주어별: m'en/t'en/s'en/nous en/vous en) | 자기도 모르게 (뿌리=se rendre compte de qch 깨닫다) | sans connaissance ❌ / 주어 se 변화 누락 | 2026-07-21 | 2026-07-26 | 11 |
| grammaire | W | devenir/venir/… = être 보조 (복합과거) | elle est devenue (+ 일치) | a devenu ❌ → est devenue | 2026-07-15 | 2026-07-16 | 0 |
| cliché | S | un média (남성, 복수 les médias) | 매체 | les nombreuses médias ❌ → nombreux | 2026-07-15 | 2026-07-16 | 0 |
| chunk | S | être en (bonne/mauvaise) forme | 컨디션이 좋다/나쁘다 | avoir mauvaise forme ❌ | 2026-07-15 | 2026-07-16 | 0 |
| cliché | S | 직업·직책은 무관사 (elle est rédactrice / PM) | être + 직업 (un/une 생략) | un rédactrice ❌ | 2026-07-15 | 2026-07-16 | 0 |
| grammaire | W | 동사 + 전치사 (à/de/sur…; sur+명사) | essayer de / se concentrer **sur+명사** / rêver de / décider de / apprendre à | essayer jouer ❌ / décide la démission ❌ | 2026-07-08 | 2026-07-16 | 3 |
| grammaire | W | depuis + 기간 + 현재 (~한 지 ~째) | J'apprends depuis 3 ans (지속) | il y a 3 ans(=~전) 혼동 | 2026-07-13 | 2026-07-14 | 0 |
| cliché | S | on dit que (사람들이 ~라고 한다) | ~라고들 한다 | on parle que ❌ | 2026-07-13 | 2026-07-14 | 0 |
| cliché | S | à + 도시 (무관사) | ~에 (도시) | au Paris ❌ → à Paris | 2026-07-13 | 2026-07-14 | 0 |
| grammaire | W | 엘리지옹 = 모음/무음h **앞에서만** (자음 앞엔 절대 X) | l'/d'/qu'/j'/n'/s'/c'/m'/t' · 자음 앞은 la/le/de 그대로 | 양방향 (7/23 워밍업 la personne·j'attends·l'horloge 3/3 정확 — 개선세) | 2026-07-07 | 2026-07-26 | 8 |
| chunk | S | petit à petit / peu à peu | 조금씩 | peu un peu ❌ | 2026-07-08 | 2026-07-09 | 0 |
| formule | W | il n'y a pas de meilleur(e) X que Y | Y보다 나은 X는 없다 | ce n'est la meilleure méthode que ❌ | 2026-07-08 | 2026-07-09 | 0 |
| chunk | S | faire les accords / lire les partitions | 코드를 잡다 / 악보를 읽다 | attraper l'accord ❌ (calque) | 2026-07-08 | 2026-07-09 | 0 |
| grammaire | W | ce qui(주어) ↔ ce que(목적어) | "~하는 것" — Ce qui + 동사, c'est + 명사 / ce que + 주어+동사 | C'est important qui… ❌ (선행사 없음) / ce que influence ❌ | 2026-07-06 | 2026-07-09 | 1 |
| chunk | S | s'entraîner à + 부정사 / pratiquer | 연습·훈련하다 (s'entraîner **à**) | exerciser ❌ / m'entraîne parler → à parler | 2026-07-07 | 2026-07-11 | 1 |
| chunk | S | faire des progrès en + 언어 | ~ 실력이 늘다 | de compétence pour ❌ (calque) | 2026-07-07 | 2026-07-08 | 0 |
| cliché | S | facilement (부사) ≠ facile (형용사) | 동사 수식은 부사 | français facile ❌ / facile séparer ❌ (재발 7/21) | 2026-07-07 | 2026-07-22 | 0 |
| chunk | W | c'est/il est + 형용사 + de + 부정사 | "~하는 것은 ~하다" (절 X, 부정사 O) | c'est facile qu'on arrive ❌ → d'arriver | 2026-07-05 | 2026-07-12 | 2 |
| chunk | S | être bon pour la santé | 건강에 좋다 | fait en bonne santé ❌ (직역) | 2026-07-06 | 2026-07-07 | 0 |
| chunk | S | une alimentation variée / des nutriments | 균형 잡힌 식단 / 영양소 | la nourritures ❌ / la riche nutrition | 2026-07-06 | 2026-07-07 | 0 |
| cliché | S | basé sur (not de) | ~에 기반한 | basé de ❌ | 2026-07-06 | 2026-07-07 | 0 |
| cliché | S | une horloge (여성) / le rythme biologique | 생체시계 | un horloge ❌ | 2026-07-06 | 2026-07-07 | 0 |
| chunk | S | ranger (정리하다) | (물건·방을) 정리 (ranger sa chambre) | arranger ❌ (재발 7/27) | 2026-07-03 | 2026-07-28 | 2 |
| chunk | S | en voiture / en train (교통수단) | 교통수단 = en + 무관사 | avec voiture ❌ → en voiture | 2026-07-05 | 2026-07-06 | 0 |
| chunk | S | profiter de | ~을 즐기다·누리다 | jouir le soleil ❌ → profiter du | 2026-07-05 | 2026-07-06 | 0 |
| chunk | S | se souvenir de / un souvenir | 기억하다 / 추억 | le memoire ❌ (=기억력·논문) | 2026-07-05 | 2026-07-06 | 0 |
| cliché | S | les vacances (항상 여성 복수) | 휴가 (de nouvelles vacances) | la nouvelle vacance ❌ | 2026-07-05 | 2026-07-06 | 0 |
| chunk | S | commander (주문하다) | 음식·물건 주문하다 | ordré ❌ (영어 order) | 2026-07-02 | 2026-07-06 | 2 |
| chunk | W | après s'être + p.p. (재귀 부정사과거) | "~한 후에" 재귀동사 (재귀대명사 유지) | après être réveillé ❌ → m'être | 2026-07-02 | 2026-07-06 | 3 |
| cliché | S | nouveau(앞)/nouvel(모음앞)/nouvelle(여) ↔ neuf(뒤, 신품) | un nouvel ordinateur / un ordinateur neuf | un neuf ordinateur ❌ | 2026-07-03 | 2026-07-12 | 1 |
| cliché | S | cette chambre (chambre 여성) | 방 (la chambre) | ce chambre ❌ | 2026-07-03 | 2026-07-04 | 0 |
| cliché | W | avoir + 앞 직목(que) → 과거분사 일치 | que j'ai achetées (chemises 여복) | que j'ai monté ❌ | 2026-07-03 | 2026-07-08 | 1 |
| chunk | W | après + avoir/être + p.p. (infinitif passé) | "~한 후에" (주절보다 선행, être면 주어 일치) | après passer ❌ / être 일치 누락(rentré→rentrée) | 2026-06-24 | 2026-07-05 | 5 |
| cliché | W | 재귀동사 복합과거 일치: se=COD→일치 / se=COI→무일치 | s'est lavée vs s'est lavé les mains / se sont parlé(à) / 본질재귀=주어일치, 예외 s'est rendu compte | "재귀=무조건 일치" 과잉일반화 | 2026-06-24 | 2026-07-05 | 3 |
| grammaire | W | quand + 미래시제 (futur) | "~할 때"(미래)는 불어는 futur | quand j'ai ❌ → j'aurai (7/3 워밍업 오답 → 작문서 정확) | 2026-07-02 | 2026-07-05 | 1 |
| chunk | S | s'entraîner à + 동사원형 | ~하는 걸 연습하다 | s'entraîner que ❌ | 2026-07-02 | 2026-07-03 | 0 |
| cliché | S | 형용사 후치 (petit-déjeuner tardif) | 대부분 형용사는 명사 뒤 | le tard petit-déjeuner ❌ | 2026-07-02 | 2026-07-03 | 0 |
| cliché | W | peu de + 가산복수 (몇 개 안 남음) | il reste peu d'épisodes | un peu de episodes reste ❌ | 2026-07-02 | 2026-07-03 | 0 |
| chunk | S | l'application de livraison | 배달 앱 | delivery app ❌ (영어) | 2026-07-02 | 2026-07-06 | 1 |
| chunk | S | il y a quelques années | 몇 년 전에 | quelque ans ❌ | 2026-07-02 | 2026-07-03 | 0 |
| cliché | S | en ville (무관사) ↔ dans la/cette ville (특정) | 일반 "도시에"=en ville / 특정 도시=dans+관사 | en cette ville ❌ (재발, en은 무관사) | 2026-06-23 | 2026-06-27 | 2 |
| chunk | W | beaucoup de + 무관사 (+ 복수면 동사 복수) | 많은 ~ (de l'argent ❌ → d'argent) | des tas de / beaucoup de l'argent / 동사 단수 ❌ | 2026-06-23 | 2026-06-25 | 1 |
| chunk | S | arriver à / dans (+ 전치사) | ~에 도착하다 | arriver la rue ❌ | 2026-06-24 | 2026-06-25 | 0 |
| chunk | S | rentrer chez soi | 귀가하다 | je vais chez moi (덜 자연) | 2026-06-24 | 2026-06-25 | 0 |
| chunk | S | sur le/mon chemin | 가는 길에 | dans mon chemin ❌ | 2026-06-24 | 2026-06-25 | 0 |
| cliché | S | prendre le déjeuner / déjeuner(동사) | 식사하다 (점심=déjeuner, 아침=petit-déjeuner) | manger le déjeuner ❌ / petit-déjeuner(아침) 혼동 | 2026-06-24 | 2026-06-25 | 0 |
| cliché | S | campagne(시골) ≠ compagne(동반자) | 철자로 뜻 바뀜 | à la compagne ❌ | 2026-06-22 | 2026-06-26 | 1 |
| cliché | S | même si + 직설법 | 양보 "설령 ~라도" | même s'il soit ❌ → est | 2026-06-22 | 2026-06-26 | 1 |
| chunk | W | en + 제롱디프 (주어 일치) | ~하면서 (en me déplaçant) | en se déplaçant ❌ (je 주어) | 2026-06-23 | 2026-06-24 | 0 |
| chunk | S | un embouteillage / embouteillé | 교통체증 / (도로가) 막힌 | "막히다" 미상 | 2026-06-23 | 2026-06-24 | 0 |
| cliché | S | le reste(나머지) ≠ les restes(남은 음식) | 단/복수로 뜻 바뀜 | les restes ❌ | 2026-06-23 | 2026-06-24 | 0 |
| cliché | S | la santé (여성) | 건강 | mon santé ❌ → ma | 2026-06-23 | 2026-06-24 | 0 |
| cliché | S | place → endroit / lieu | 장소 (place=광장·자리) | place 오용 | 2026-06-22 | 2026-06-25 | 0 |
| cliché | S | chercher → trouver / aller | 찾다 ≠ 가다·이용 | chercher 남용 | 2026-06-22 | 2026-06-25 | 0 |
| chunk | W | tout ce dont / ce que | ~하는 (모든) 것 | 관계대명사 누락 | 2026-06-22 | 2026-06-25 | 0 |
| connecteur | W | Premièrement / Deuxièmement / Enfin | 첫째/둘째/마지막 | En premier·seconde ❌ | 2026-06-22 | 2026-07-08 | 1 |
| chunk | S | transports en commun | 대중교통 | La transport ❌ / des tas de transport ❌ | 2026-06-22 | 2026-06-26 | 1 |
| cliché | S | S'il (엘리지옹) | Si + il → S'il | Si il ❌ (재발) | 2026-06-22 | 2026-06-25 | 0 |
| chunk | W | préférer A plutôt que B | A를 B보다 선호 | plus vivre que ❌ / plutôt que à → qu'à | 2026-06-22 | 2026-07-08 | 1 |
| chunk | S | jouer à + 게임 | (게임)을 하다 | faire le jeu ❌ / jouer Overwatch ❌ | 2026-06-22 | 2026-07-06 | 1 |
| chunk | W | un entraînement à l'écriture | 작문 훈련 | s'exercer 작문 ❌ | 2026-06-22 | 2026-06-25 | 0 |
| chunk | S | pour progresser | 실력을 늘리려고 | — | 2026-06-22 | 2026-06-25 | 0 |
| cliché | S | quelque chose (불변 단수) | 무언가 | quelque choses ❌ | 2026-06-22 | 2026-06-25 | 0 |
| chunk | S | un personnage de soutien | 서포터 (게임 역할) | l'assistant position ❌ | 2026-06-22 | 2026-06-25 | 0 |
| chunk | S | soigner ses coéquipiers | 팀원을 치료하다 | récupérer la forme ❌ | 2026-06-22 | 2026-06-25 | 0 |
| formule | S | Ce qui me séduit, c'est… | 내가 매력 느끼는 건 ~ (강조 분열문) | que je suis charmé ❌ | 2026-06-22 | 2026-06-25 | 0 |
| cliché | S | utiliser (not utilize) / on peut | 사용하다 / 활용 | 영어혼용 + on peux | 2026-06-22 | 2026-06-25 | 0 |
| cliché | S | en dehors de | ~밖에·외부에 | dehors Buzzvil ❌ | 2026-06-22 | 2026-06-25 | 0 |
| cliché | S | chercher sur Internet | 인터넷에서 검색하다 | rechercher l'internet ❌ | 2026-06-22 | 2026-06-25 | 0 |
| formule | S | Je veux dire… / C'est dommage | 내 말은~ / 아쉽다 | (잘 씀, 강화) | 2026-06-22 | 2026-06-25 | 0 |

## T3 — 간격 반복 (정착)

| 카테고리 | reg | 표현/패턴 | 의미·용법 | 흔한 오류 | 정착일 | 다음 복습일 | 단계 |
|---|---|---|---|---|---|---|---|
| grammaire | W | comme si + 반과거(현재 비현실)/대과거(과거 비현실) | comme s'il était millionnaire / comme si j'avais gagné · 대과거 aux 주의(rencontrer=avoir) | comme si + 현재·PC ❌ (7/21 n'a compris→n'avait) | 2026-07-18 | 2026-07-24 | 3일 |

## T4 — 참조 보관 (능동 학습 X)

| 카테고리 | reg | 표현/패턴 | 의미·용법 | 흔한 오류 | 발견일 | 비고 |
|---|---|---|---|---|---|---|
| cliché | S | insectes (not insects) | 곤충 | 영어 혼용 | 2026-06-22 | 단발 |
| chunk | S | se déplacer | 이동하다 | (자연 표현) | 2026-06-22 | 참조 |
| chunk | S | tout près | 바로 가까이 | (자연 표현) | 2026-06-22 | 참조 |
| cliché | S | le français (남성) | 프랑스어 | la français ❌ | 2026-06-23 | 향후 자동 해소 |
| cliché | S | populaire (not popular) | 인기 있는/대중적 | popular ❌ (영어 혼용) | 2026-06-24 | 단발 |
| chunk | S | une rue gourmande / des restaurants | 맛집 거리 | rue de goût ❌ | 2026-06-24 | 참조 |
| chunk | S | le sirop d'érable | 메이플 시럽 | maple syrop ❌ (영어) | 2026-07-02 | 단발 |
| chunk | S | monter / assembler (un meuble), une vis / un boulon | 가구 조립 / 나사·볼트 | 조립·볼트 (한국어) | 2026-07-02 | 참조 |
| chunk | S | cette nuit / ce soir | 오늘 밤 / 오늘 저녁 | dans la nuit d'aujourd'hui ❌ | 2026-07-03 | 참조 |
| chunk | S | le grand large | 넓은 바다·먼바다 | le grand monde ❌ (=사교계) | 2026-07-05 | 참조 |
| cliché | S | large (넓은) ≠ 영어 large(큰) | 큰=grand / 넓은=large | faux-ami (large=크다 오해) | 2026-07-05 | 참조 |
| chunk | S | les hormones / le système immunitaire | 호르몬 / 면역계 | hormones de l'immunité (어색) | 2026-07-06 | 참조 |
| chunk | S | surfer sur les vagues | 파도를 타다 | surfer sur le mouvement ❌ | 2026-07-05 | 참조 |
| chunk | S | grimper / monter (une montagne) | (산을) 오르다 | assensionner ❌ (없는 말) | 2026-07-05 | 참조 |
| chunk | S | un système d'alerte de stock | 재고 알림 시스템 | système d'alarme ❌ | 2026-07-18 | 참조 |
| chunk | S | un magasin physique | 오프라인 매장 | magasin hors ligne ❌ (calque) | 2026-07-18 | 참조 |
| chunk | S | la détaxe / un jour férié | 면세 / 공휴일 | détaxé ❌ | 2026-07-18 | 참조 |
| cliché | S | une console (여성) | 게임기 | il est (console) ❌ → elle | 2026-07-18 | 참조 |
| chunk | S | une navette (du campus) | 순환 셔틀버스 | bus circulaire ❌ | 2026-07-19 | 참조 |
| chunk | S | une résidence universitaire | (대학) 기숙사 | pension universitaire ❌ | 2026-07-19 | 참조 |
| chunk | S | en bas ↔ en haut | 아래쪽 ↔ 위쪽 | la bas/la haut ❌ | 2026-07-19 | 참조 |
| chunk | S | avoir l'impression de + 부정사 | ~한 기분이 들다 | avoir l'air d'être un coup de poing ❌ | 2026-07-19 | 참조 |
| cliché | S | un parapluie (남성) | 우산 | la parapluie ❌ | 2026-07-20 | 참조 |
| cliché | S | difficulté (이중 f) | 어려움 | dificulté ❌ | 2026-07-20 | 참조 |
| cliché | S | le moral / le bien-être (≠ la mentalité) | 정신 건강·기분 | mieux pour ma mentalité ❌ | 2026-07-21 | 참조 |
| cliché | S | bleu (철자) / le ciel bleu | 파란 | blue ❌ (영어) | 2026-07-21 | 참조 |
| cliché | S | une attente (기대) ≠ attendre (기다리다) | les attentes des autres | l'attendre d'autre ❌ | 2026-07-24 | 참조 |
| cliché | S | indéfiniment (무한정) | 계속·끝없이 | infinitement ❌ | 2026-07-24 | 참조 |
| cliché | S | une fonction / une fonctionnalité (여성) | 기능 | le nouvel fonction ❌ → une nouvelle | 2026-07-25 | 참조 |
| chunk | S | les réseaux sociaux (un réseau social) | SNS·소셜 미디어 (≠ les médias 매체) | (단어 미상) | 2026-07-25 | 참조 |
| chunk | W | balbutier quelques mots | 몇 마디 더듬거리다 | (잘 씀, 고급) | 2026-07-25 | 참조 |
| chunk | S | avoir l'air de + 부정사 / + 형용사 | ~해 보이다 (il a l'air de dormir / fatigué) | (잘 씀) | 2026-07-27 | 참조 |
| grammaire | W | 부사 bien은 부정사 앞 (bien peindre) | 어순 | peindre bien ❌ | 2026-07-27 | 참조 |

---

## 사전 풀 (Q3 시작 시 베이스라인 자가 분류 → T1\~T4 배치)

> 5/1 작문 시범 결과 + 핵심 정형표현. Q3 시작 시 사용자가 "이미 능동/반복 필요/모름"으로 자가 분류하면 그게 베이스라인이 되고, 카드가 T1\~T4로 흩어진다.

### chunk (collocation)

| reg | 표현 | 의미 | 흔한 오류 |
|---|---|---|---|
| S | en terrasse | 카페 야외석에 | ~~à la terrasse~~ ⭐ 5/1 큰 수확 |
| S | prendre une décision | 결정을 내리다 | ~~faire une décision~~ |
| S | faire la queue | 줄을 서다 | |
| S | prendre une photo | 사진을 찍다 | |
| S | passer un examen | 시험을 보다 | ~~voir un examen~~ |
| S | tomber dans les pommes | 기절하다 | (단발성 → T4 후보) |

### cliché (한국어 화자 함정) — 5/1 시범 13개

| reg | 정답/회피 | 함정 | 비고 |
|---|---|---|---|
| S | offrir (호의·선물) | ~~donner~~ | ⭐⭐ 한 세션 2회 등장 — T1 1순위 |
| S | donner/raconter qch **à qqn** | 수령자 누락 | "주다/말하다" 직역 |
| S | depuis(지속) ↔ il y a(시점) | 혼동 | 시간 표현 핵심 |
| S | son + 모음명사 | ~~sa + 모음~~ | 발음 hiatus 회피 |
| W/S | en + gérondif / pendant + 명사 | ~~pendant + 동사원형~~ | 강한 직역 함정 |
| S | 명사 직접 목적어 | l'histoire de… 풀어쓰기 | "X의 이야기" → "X" |
| S | arriver / être servi (음식) | ~~sortir~~ | 동사 선택 |
| S | personnage / thé / heure | character / téa / hour | 영어 혼용 → T4 |
| W | avec X écrit dessus | qui est écrit… | 관계절 어색 구조 |

### formule (정형표현 6카테고리)

| reg | 표현 | 기능 |
|---|---|---|
| W | Pour ma part, je pense que… | 의견 |
| S | Il me semble que… | 인상 |
| W | Cela dit, … | 양보 |
| S | En revanche, … | 대조 |
| W | En somme, … | 요약 |
| S | Ce qui m'intéresse, c'est… | 강조 |
| S | Ça fait + 기간 + que + 절 | "~한 지 ~됐다" ⭐ 5/1 수확 |

### connecteur (연결사)

| reg | 표현 | 단계 |
|---|---|---|
| S | donc / alors | A2\~B1 |
| W | en effet / par ailleurs | B1\~B2 |
| W | néanmoins / cependant | B1\~B2 |
| W | en dépit de / faute de | C1 |

---

## 통계 (주 1회 /write 자동 산출)

> 신규 chunk 수 / Tier 이동(T2→T3 정착) / 활용 빈도 / 활용 미달(사용 권장) 등.
> **회사 공유 = 매달 1,500단어 (양적만, 6/22 확정).** 질적(rubric DELF B1 6항목)·chunk는 **내부 측정/방향타 도구** (회사 공유 X).
