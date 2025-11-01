# ssdsDASD
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>اختبار خواص المادة التفاعلي</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
            background-color: #f5f5f5;
            color: #333;
        }
        .container {
            background-color: white;
            border-radius: 10px;
            padding: 30px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }
        h1 {
            text-align: center;
            color: #2c3e50;
            margin-bottom: 30px;
            border-bottom: 2px solid #3498db;
            padding-bottom: 10px;
        }
        .section-title {
            background-color: #3498db;
            color: white;
            padding: 10px;
            border-radius: 5px;
            margin: 25px 0 15px;
            text-align: center;
        }
        .question {
            margin-bottom: 25px;
            padding: 15px;
            border-radius: 8px;
            background-color: #f9f9f9;
            border-left: 4px solid #3498db;
        }
        .question-number {
            font-weight: bold;
            color: #2c3e50;
            margin-bottom: 8px;
        }
        .options {
            margin-top: 10px;
        }
        .option {
            margin-bottom: 8px;
            padding: 8px;
            border-radius: 5px;
            transition: background-color 0.3s;
        }
        .option:hover {
            background-color: #eef7ff;
        }
        .option input {
            margin-left: 10px;
        }
        .option label {
            cursor: pointer;
            display: block;
            padding: 5px 10px;
        }
        .correct-answer {
            background-color: #d4edda;
            border: 1px solid #c3e6cb;
            color: #155724;
            padding: 10px;
            border-radius: 5px;
            margin-top: 10px;
            display: none;
        }
        .submit-btn {
            display: block;
            width: 200px;
            margin: 30px auto;
            padding: 12px;
            background-color: #3498db;
            color: white;
            border: none;
            border-radius: 5px;
            font-size: 16px;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        .submit-btn:hover {
            background-color: #2980b9;
        }
        .results {
            text-align: center;
            margin-top: 30px;
            padding: 20px;
            border-radius: 10px;
            background-color: #e8f4fc;
            display: none;
        }
        .score {
            font-size: 24px;
            font-weight: bold;
            color: #2c3e50;
            margin: 15px 0;
        }
        .footer {
            text-align: center;
            margin-top: 30px;
            padding-top: 15px;
            border-top: 1px solid #ddd;
            color: #7f8c8d;
        }
        .progress-bar {
            height: 10px;
            background-color: #ecf0f1;
            border-radius: 5px;
            margin-bottom: 20px;
            overflow: hidden;
        }
        .progress {
            height: 100%;
            background-color: #3498db;
            width: 0%;
            transition: width 0.5s;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>اختبار خواص المادة التفاعلي</h1>
        
        <div class="progress-bar">
            <div class="progress" id="progress"></div>
        </div>
        
        <form id="quiz-form">
            <div class="section-title">حالات المادة</div>
            
            <div class="question">
                <div class="question-number">1. أي مما يلي يُعدّ من حالات المادة الأساسية؟</div>
                <div class="options">
                    <div class="option">
                        <label>
                            <input type="radio" name="q1" value="a"> (أ) البلازما
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q1" value="b"> (ب) الصلبة
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q1" value="c"> (ج) الغروبة
                        </label>
                    </div>
                </div>
                <div class="correct-answer" id="answer1">الإجابة الصحيحة: (ب) الصلبة</div>
            </div>
            
            <div class="question">
                <div class="question-number">2. أي خاصية تُميز المادة الصلبة؟</div>
                <div class="options">
                    <div class="option">
                        <label>
                            <input type="radio" name="q2" value="a"> (أ) ليس لها حجم ثابت
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q2" value="b"> (ب) لها شكل ثابت
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q2" value="c"> (ج) تنضغط بسهولة
                        </label>
                    </div>
                </div>
                <div class="correct-answer" id="answer2">الإجابة الصحيحة: (ب) لها شكل ثابت</div>
            </div>
            
            <div class="question">
                <div class="question-number">3. أي مما يلي يُعدّ من خصائص السوائل؟</div>
                <div class="options">
                    <div class="option">
                        <label>
                            <input type="radio" name="q3" value="a"> (أ) شكل ثابت
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q3" value="b"> (ب) حجم ثابت
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q3" value="c"> (ج) يمكن ضغطها بشدة
                        </label>
                    </div>
                </div>
                <div class="correct-answer" id="answer3">الإجابة الصحيحة: (ب) حجم ثابت</div>
            </div>
            
            <div class="question">
                <div class="question-number">4. الغازات تتميز بأنها؟</div>
                <div class="options">
                    <div class="option">
                        <label>
                            <input type="radio" name="q4" value="a"> (أ) لها شكل وحجم ثابت
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q4" value="b"> (ب) ليس لها شكل أو حجم ثابت
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q4" value="c"> (ج) لا تتحرك جسيماتها
                        </label>
                    </div>
                </div>
                <div class="correct-answer" id="answer4">الإجابة الصحيحة: (ب) ليس لها شكل أو حجم ثابت</div>
            </div>
            
            <div class="question">
                <div class="question-number">5. أي مما يلي مثال على بخار؟</div>
                <div class="options">
                    <div class="option">
                        <label>
                            <input type="radio" name="q5" value="a"> (أ) بخار الماء
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q5" value="b"> (ب) غاز الأكسجين
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q5" value="c"> (ج) غاز ثاني أكسيد الكربون
                        </label>
                    </div>
                </div>
                <div class="correct-answer" id="answer5">الإجابة الصحيحة: (أ) بخار الماء</div>
            </div>
            
            <div class="section-title">الخواص الفيزيائية والكيميائية</div>
            
            <div class="question">
                <div class="question-number">6. أي خاصية يمكن ملاحظتها دون تغيير تركيب المادة؟</div>
                <div class="options">
                    <div class="option">
                        <label>
                            <input type="radio" name="q6" value="a"> (أ) فيزيائية
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q6" value="b"> (ب) كيميائية
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q6" value="c"> (ج) نوية
                        </label>
                    </div>
                </div>
                <div class="correct-answer" id="answer6">الإجابة الصحيحة: (أ) فيزيائية</div>
            </div>
            
            <div class="question">
                <div class="question-number">7. أي من الخواص التالية تُعدّ خاصية فيزيائية؟</div>
                <div class="options">
                    <div class="option">
                        <label>
                            <input type="radio" name="q7" value="a"> (أ) الكثافة
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q7" value="b"> (ب) التفاعل مع الأحماض
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q7" value="c"> (ج) الاشتعال
                        </label>
                    </div>
                </div>
                <div class="correct-answer" id="answer7">الإجابة الصحيحة: (أ) الكثافة</div>
            </div>
            
            <div class="question">
                <div class="question-number">8. أي من الخواص التالية تُعدّ خاصية كيميائية؟</div>
                <div class="options">
                    <div class="option">
                        <label>
                            <input type="radio" name="q8" value="a"> (أ) القابلية للاشتعال
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q8" value="b"> (ب) الكتلة
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q8" value="c"> (ج) الطول
                        </label>
                    </div>
                </div>
                <div class="correct-answer" id="answer8">الإجابة الصحيحة: (أ) القابلية للاشتعال</div>
            </div>
            
            <div class="question">
                <div class="question-number">9. الكثافة تُعدّ من الخواص؟</div>
                <div class="options">
                    <div class="option">
                        <label>
                            <input type="radio" name="q9" value="a"> (أ) الشدة
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q9" value="b"> (ب) الممتدة
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q9" value="c"> (ج) الكيميائية
                        </label>
                    </div>
                </div>
                <div class="correct-answer" id="answer9">الإجابة الصحيحة: (أ) الشدة</div>
            </div>
            
            <div class="question">
                <div class="question-number">10. الطول يُعدّ من الخواص:</div>
                <div class="options">
                    <div class="option">
                        <label>
                            <input type="radio" name="q10" value="a"> (أ) نوعية
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q10" value="b"> (ب) كمية
                        </label>
                    </div>
                    <div class="option">
                        <label>
                            <input type="radio" name="q10" value="c"> (ج) كيميائية
                        </label>
                    </div>
                </div>
                <div class="correct-answer" id="answer10">الإجابة الصحيحة: (ب) كمية</div>
            </div>
            
            <!-- يمكن إضافة المزيد من الأسئلة هنا -->
            
            <button type="button" class="submit-btn" id="submit-btn">تقديم الإجابات</button>
        </form>
        
        <div class="results" id="results">
            <h2>نتيجة الاختبار</h2>
            <div class="score" id="score">0/10</div>
            <p id="result-message"></p>
            <button type="button" class="submit-btn" id="retry-btn">إعادة الاختبار</button>
        </div>
        
        <div class="footer">
            <p>تم إنشاء هذا الاختبار بناءً على ملف Document 9.pdf</p>
        </div>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const form = document.getElementById('quiz-form');
            const submitBtn = document.getElementById('submit-btn');
            const results = document.getElementById('results');
            const scoreElement = document.getElementById('score');
            const resultMessage = document.getElementById('result-message');
            const retryBtn = document.getElementById('retry-btn');
            const progress = document.getElementById('progress');
            
            // الإجابات الصحيحة
            const correctAnswers = {
                q1: 'b',
                q2: 'b',
                q3: 'b',
                q4: 'b',
                q5: 'a',
                q6: 'a',
                q7: 'a',
                q8: 'a',
                q9: 'a',
                q10: 'b'
                // يمكن إضافة المزيد من الإجابات الصحيحة هنا
            };
            
            // تحديث شريط التقدم
            function updateProgress() {
                const totalQuestions = Object.keys(correctAnswers).length;
                let answered = 0;
                
                for (const question in correctAnswers) {
                    if (form.elements[question].value) {
                        answered++;
                    }
                }
                
                const progressPercent = (answered / totalQuestions) * 100;
                progress.style.width = `${progressPercent}%`;
            }
            
            // إضافة مستمعات الأحداث لأسئلة الاختبار
            for (const question in correctAnswers) {
                const inputs = document.querySelectorAll(`input[name="${question}"]`);
                inputs.forEach(input => {
                    input.addEventListener('change', updateProgress);
                });
            }
            
            // تقديم الإجابات
            submitBtn.addEventListener('click', function() {
                let score = 0;
                const totalQuestions = Object.keys(correctAnswers).length;
                
                // حساب النتيجة
                for (const question in correctAnswers) {
                    const selectedOption = form.elements[question].value;
                    const correctAnswer = correctAnswers[question];
                    
                    if (selectedOption === correctAnswer) {
                        score++;
                    }
                    
                    // عرض الإجابات الصحيحة
                    if (selectedOption) {
                        document.getElementById(`answer${question.substring(1)}`).style.display = 'block';
                    }
                }
                
                // عرض النتيجة
                scoreElement.textContent = `${score}/${totalQuestions}`;
                
                // رسالة النتيجة
                const percentage = (score / totalQuestions) * 100;
                if (percentage >= 80) {
                    resultMessage.textContent = 'ممتاز! أداء رائع.';
                    resultMessage.style.color = '#27ae60';
                } else if (percentage >= 60) {
                    resultMessage.textContent = 'جيد، لكن يمكنك التحسين.';
                    resultMessage.style.color = '#f39c12';
                } else {
                    resultMessage.textContent = 'يجب مراجعة المادة الدراسية.';
                    resultMessage.style.color = '#e74c3c';
                }
                
                results.style.display = 'block';
                submitBtn.style.display = 'none';
                
                // التمرير إلى النتيجة
                results.scrollIntoView({ behavior: 'smooth' });
            });
            
            // إعادة الاختبار
            retryBtn.addEventListener('click', function() {
                form.reset();
                results.style.display = 'none';
                submitBtn.style.display = 'block';
                
                // إخفاء الإجابات الصحيحة
                for (let i = 1; i <= Object.keys(correctAnswers).length; i++) {
                    document.getElementById(`answer${i}`).style.display = 'none';
                }
                
                // إعادة تعيين شريط التقدم
                progress.style.width = '0%';
                
                // التمرير إلى الأعلى
                window.scrollTo({ top: 0, behavior: 'smooth' });
            });
        });
    </script>
</body>
</html>
