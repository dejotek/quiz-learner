# Quiz Learner

### Platforma do nauki z gotowymi bazami oraz kreatorem quizów.



## Struktura plików w projekcie

src/
│
├── app/
│   ├── App.tsx
│   ├── App.css
│   └── routes.tsx
│
├── assets/
│   ├── images/
│   ├── icons/
│   └── styles/
│       ├── variables.css
│       └── global.css
│
├── components/
│   ├── common/
│   │   ├── Button/
│   │   │   ├── Button.tsx
│   │   │   └── Button.css
│   │   ├── Loader/
│   │   └── Modal/
│   │
│   └── layout/
│       ├── Header/
│       ├── Footer/
│       └── PageWrapper/
│
├── features/
│   ├── auth/
│   │   ├── LoginPage.tsx
│   │   ├── RegisterPage.tsx
│   │   └── auth.service.ts
│   │
│   ├── quizzes/
│   │   ├── QuizListPage.tsx
│   │   ├── QuizPage.tsx
│   │   ├── QuizResultPage.tsx
│   │   ├── quiz.types.ts
│   │   └── quiz.service.ts
│   │
│   ├── questions/
│   │   ├── QuestionCard.tsx
│   │   ├── AnswerOption.tsx
│   │   └── question.types.ts
│   │
│   └── profile/
│       ├── ProfilePage.tsx
│       └── profile.service.ts
│
├── hooks/
│   ├── useAuth.ts
│   ├── useQuiz.ts
│   └── useTimer.ts
│
├── services/
│   ├── api.ts
│   └── storage.ts
│
├── store/
│   ├── index.ts
│   └── quiz.store.ts
│
├── types/
│   └── common.ts
│
├── utils/
│   ├── shuffleArray.ts
│   ├── formatTime.ts
│   └── calculateScore.ts
│
├── index.tsx
├── index.css
└── react-app-env.d.ts

