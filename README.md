import React, { useMemo, useState } from "react";
import { motion } from "framer-motion";
import { Rocket, Target, Users, ShieldCheck, BarChart3, CheckCircle2, ArrowRight, Sparkles, ClipboardList, MessageCircle, Search, CalendarCheck, UserCheck, ChevronRight } from "lucide-react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";

const rSteps = [
  { id: "R1", title: "取得名單", icon: ClipboardList, desc: "建立緣故名單、推薦人名單，找到增員起點。" },
  { id: "R2", title: "啟動接觸", icon: Users, desc: "運用行為模式與定聯分級，讓接觸更自然。" },
  { id: "R3", title: "發掘需求", icon: Search, desc: "透過六大面向提問，找到準增真正重視的工作條件。" },
  { id: "R4", title: "邀約推進", icon: CalendarCheck, desc: "用 FAB 邀約法，把聊天推進到下一步行動。" },
  { id: "R5", title: "面談追蹤", icon: MessageCircle, desc: "處理異議、釐清卡點，讓準增願意繼續往下走。" },
  { id: "R6", title: "新人報聘", icon: UserCheck, desc: "把增員流程收斂到結果，完成新人報聘與起步陪跑。" },
];

const painPoints = [
  "想增員，卻不知道從哪裡開始",
  "有名單，卻不知道怎麼接觸與往下推",
  "會聊天，卻不一定能發掘準增需求",
  "邀約常卡住，異議來了不知如何處理",
  "想把增員做穩，卻缺少完整方法與節奏",
];

const courses = [
  {
    name: "主任經典基礎班",
    focus: "聚焦增員起步與基本功建立",
    range: "打穩 R1～R2 基礎能力",
    icon: ShieldCheck,
    items: ["看懂 R 線全貌", "建立緣故名單與推薦人名單", "掌握增員定聯分級", "運用行為模式測驗開啟接觸", "邀約準增參加活動", "補強退休、稅務、保障等行銷切入點"],
  },
  {
    name: "主任進階班",
    focus: "聚焦需求挖掘與推進能力",
    range: "強化 R2～R4 關鍵做法",
    icon: Target,
    items: ["網路增員與陌生開發", "發掘準增需求與六大面向提問", "FAB 邀約法與邀約下一步", "異議問題處理", "建立活動量管理與穩定增員節奏"],
  },
];

const outcomeCards = [
  { title: "角色更到位", desc: "清楚知道晉升後，每個階段該做什麼。", icon: ShieldCheck },
  { title: "行銷有方向", desc: "不只會做業績，也懂得用議題切入市場。", icon: Target },
  { title: "增員有方法", desc: "從名單、接觸、需求、邀約到推進，知道如何往下走。", icon: Users },
  { title: "習慣能落地", desc: "不再只靠感覺增員，而是建立可持續的節奏與方法。", icon: BarChart3 },
];

const quizQuestions = [
  { q: "我現在最常卡在：", options: ["不知道名單從哪來", "有名單但不敢接觸", "聊得起來但推不下去", "邀約或異議處理卡住"] },
  { q: "我最想補強的是：", options: ["建立完整增員流程", "提升接觸與邀約能力", "發掘準增需求", "建立穩定增員節奏"] },
  { q: "目前我的增員狀態比較像：", options: ["知道重要，但還沒開始", "偶爾做，但不穩定", "有行動，但缺方法", "想做出固定成果"] },
];

export default function DirectorTrainingLandingPage() {
  const [activeStep, setActiveStep] = useState(0);
  const [answers, setAnswers] = useState({});
  const [showResult, setShowResult] = useState(false);

  const result = useMemo(() => {
    const values = Object.values(answers);
    if (values.length < 3) return "";
    if (values.some((v) => String(v).includes("名單") || String(v).includes("開始"))) return "建議優先從主任經典基礎班開始，先打穩 R1～R2 的名單、接觸與邀約基本功。";
    if (values.some((v) => String(v).includes("需求") || String(v).includes("異議") || String(v).includes("推"))) return "建議聚焦主任進階班，強化 R2～R4 的需求挖掘、FAB邀約與異議處理能力。";
    return "建議兩班銜接學習，從流程、方法到節奏完整建立，讓增員變成可持續行動。";
  }, [answers]);

  const ActiveIcon = rSteps[activeStep].icon;

  return (
    <div className="min-h-screen bg-[#06142f] text-white overflow-hidden">
      <div className="absolute inset-0 opacity-40 bg-[radial-gradient(circle_at_20%_20%,#1e88ff_0,transparent_28%),radial-gradient(circle_at_80%_10%,#ff9f1c_0,transparent_22%),linear-gradient(135deg,#06142f,#071b44_45%,#020817)]" />
      <div className="absolute inset-0 opacity-20" style={{ backgroundImage: "linear-gradient(90deg, rgba(255,255,255,.08) 1px, transparent 1px), linear-gradient(rgba(255,255,255,.08) 1px, transparent 1px)", backgroundSize: "48px 48px" }} />

      <main className="relative z-10 mx-auto max-w-6xl px-5 py-8 md:py-12">
        <section className="grid items-center gap-8 md:grid-cols-[1.08fr_.92fr]">
          <motion.div initial={{ opacity: 0, y: 24 }} animate={{ opacity: 1, y: 0 }} transition={{ duration: 0.7 }}>
            <div className="inline-flex items-center gap-2 rounded-full border border-amber-300/60 bg-amber-400/10 px-4 py-2 text-sm font-semibold text-amber-200 shadow-lg shadow-amber-500/10">
              <Sparkles size={16} /> 主任必修課程
            </div>
            <h1 className="mt-6 text-5xl font-black leading-tight tracking-tight md:text-7xl">
              晉升後 <span className="bg-gradient-to-r from-amber-200 to-orange-500 bg-clip-text text-transparent">3～6個月</span>
              <br />增員培訓課程
            </h1>
            <p className="mt-5 text-xl font-bold text-amber-200 md:text-2xl">以 R 線為主軸，打造主任增員實戰力</p>
            <p className="mt-5 max-w-2xl text-base leading-8 text-blue-50/90 md:text-lg">
              晉升主任後，真正的挑戰不只是延續個人業績，而是開始面對增員、推進增員，並建立屬於自己的增員節奏。這堂課以公司 R 線增員流程為主軸，幫助你從「會做業務」走向「會推進增員」。
            </p>
            <div className="mt-7 rounded-2xl border border-amber-300/70 bg-gradient-to-r from-amber-500/20 to-orange-500/20 px-5 py-4 text-xl font-black text-amber-100 shadow-xl shadow-orange-500/20">
              把增員從「知道重要」，變成「知道怎麼做」
            </div>
          </motion.div>

          <motion.div initial={{ opacity: 0, scale: 0.92 }} animate={{ opacity: 1, scale: 1 }} transition={{ duration: 0.7, delay: 0.1 }} className="relative">
            <div className="absolute -inset-6 rounded-full bg-orange-400/20 blur-3xl" />
            <Card className="relative border-blue-300/30 bg-white/10 shadow-2xl shadow-blue-950/40 backdrop-blur-xl">
              <CardContent className="p-7">
                <div className="flex items-center justify-between">
                  <div>
                    <p className="text-sm font-semibold text-blue-100/80">課程核心流程</p>
                    <h2 className="text-3xl font-black text-white">R1 → R6</h2>
                  </div>
                  <Rocket className="text-amber-300" size={58} />
                </div>
                <div className="mt-6 space-y-3">
                  {rSteps.map((step, idx) => (
                    <button key={step.id} onClick={() => setActiveStep(idx)} className={`w-full rounded-2xl border px-4 py-3 text-left transition ${activeStep === idx ? "border-amber-300 bg-amber-300/20 shadow-lg shadow-amber-500/10" : "border-white/15 bg-white/5 hover:bg-white/10"}`}>
                      <div className="flex items-center gap-3">
                        <span className="rounded-xl bg-blue-950 px-3 py-1 font-black text-amber-300">{step.id}</span>
                        <span className="font-bold text-white">{step.title}</span>
                        <ChevronRight className="ml-auto text-blue-100/70" size={18} />
                      </div>
                    </button>
                  ))}
                </div>
              </CardContent>
            </Card>
          </motion.div>
        </section>

        <section className="mt-10 rounded-3xl border border-white/15 bg-white/10 p-5 backdrop-blur-xl md:p-8">
          <div className="grid items-center gap-6 md:grid-cols-[.85fr_1.15fr]">
            <div className="rounded-3xl bg-gradient-to-br from-blue-500/25 to-orange-500/20 p-6">
              <ActiveIcon className="text-amber-300" size={56} />
              <div className="mt-4 text-5xl font-black text-amber-300">{rSteps[activeStep].id}</div>
              <h3 className="mt-2 text-3xl font-black">{rSteps[activeStep].title}</h3>
              <p className="mt-4 text-lg leading-8 text-blue-50/90">{rSteps[activeStep].desc}</p>
            </div>
            <div>
              <h2 className="text-3xl font-black">為什麼要上這堂課？</h2>
              <p className="mt-2 text-blue-100/80">很多新晉升主任不是不想增員，而是缺少一套可執行的流程與節奏。</p>
              <div className="mt-5 grid gap-3">
                {painPoints.map((item, idx) => (
                  <div key={item} className="flex items-center gap-3 rounded-2xl border border-blue-200/20 bg-white/10 px-4 py-3">
                    <span className="flex h-8 w-8 items-center justify-center rounded-full bg-amber-400 font-black text-blue-950">{idx + 1}</span>
                    <span className="font-semibold">{item}</span>
                  </div>
                ))}
              </div>
            </div>
          </div>
        </section>

        <section className="mt-10">
          <div className="mb-5 flex items-end justify-between gap-4">
            <div>
              <p className="font-bold text-amber-200">主任經典基礎班 × 主任進階班</p>
              <h2 className="text-4xl font-black">你可以學到什麼</h2>
            </div>
          </div>
          <div className="grid gap-5 md:grid-cols-2">
            {courses.map((course) => {
              const Icon = course.icon;
              return (
                <Card key={course.name} className="border-white/20 bg-white text-slate-950 shadow-2xl">
                  <CardContent className="p-7">
                    <div className="flex items-start gap-4">
                      <div className="rounded-2xl bg-gradient-to-br from-amber-300 to-orange-500 p-3 text-white shadow-lg">
                        <Icon size={34} />
                      </div>
                      <div>
                        <h3 className="text-3xl font-black text-blue-950">{course.name}</h3>
                        <p className="mt-1 font-bold text-orange-600">{course.focus}</p>
                        <p className="text-sm font-semibold text-slate-500">{course.range}</p>
                      </div>
                    </div>
                    <div className="mt-6 space-y-3">
                      {course.items.map((item) => (
                        <div key={item} className="flex gap-3 rounded-2xl bg-blue-50 px-4 py-3 font-semibold text-slate-700">
                          <CheckCircle2 className="shrink-0 text-orange-500" size={20} />
                          {item}
                        </div>
                      ))}
                    </div>
                  </CardContent>
                </Card>
              );
            })}
          </div>
        </section>

        <section className="mt-10 grid gap-5 md:grid-cols-4">
          {outcomeCards.map((card) => {
            const Icon = card.icon;
            return (
              <Card key={card.title} className="border-white/15 bg-white/10 backdrop-blur-xl transition hover:-translate-y-1 hover:bg-white/15">
                <CardContent className="p-6">
                  <Icon className="text-amber-300" size={36} />
                  <h3 className="mt-4 text-2xl font-black text-white">{card.title}</h3>
                  <p className="mt-3 leading-7 text-blue-50/85">{card.desc}</p>
                </CardContent>
              </Card>
            );
          })}
        </section>

        <section className="mt-10 grid gap-6 md:grid-cols-[1fr_1fr]">
          <Card className="border-amber-300/40 bg-gradient-to-br from-white to-blue-50 text-slate-950 shadow-2xl">
            <CardContent className="p-7">
              <h2 className="text-3xl font-black text-blue-950">30 秒找出你的增員卡點</h2>
              <p className="mt-2 text-slate-600">選完三題，系統會建議你更適合優先補強的課程方向。</p>
              <div className="mt-6 space-y-6">
                {quizQuestions.map((q, qIdx) => (
                  <div key={q.q}>
                    <p className="mb-3 font-black text-slate-800">{qIdx + 1}. {q.q}</p>
                    <div className="grid gap-2">
                      {q.options.map((option) => (
                        <button key={option} onClick={() => setAnswers({ ...answers, [qIdx]: option })} className={`rounded-xl border px-4 py-3 text-left font-semibold transition ${answers[qIdx] === option ? "border-orange-500 bg-orange-50 text-orange-700" : "border-slate-200 bg-white hover:border-blue-300"}`}>
                          {option}
                        </button>
                      ))}
                    </div>
                  </div>
                ))}
              </div>
              <Button onClick={() => setShowResult(true)} className="mt-6 w-full rounded-2xl bg-gradient-to-r from-orange-500 to-amber-400 py-6 text-lg font-black text-blue-950 hover:opacity-90">
                查看建議課程 <ArrowRight className="ml-2" size={20} />
              </Button>
            </CardContent>
          </Card>

          <Card className="border-white/15 bg-white/10 backdrop-blur-xl">
            <CardContent className="flex h-full flex-col justify-between p-7">
              <div>
                <p className="font-bold text-amber-200">適合對象</p>
                <h2 className="mt-1 text-4xl font-black">新晉升主任 3～6 個月內</h2>
                <p className="mt-5 text-lg leading-8 text-blue-50/85">
                  這不只是一門課，而是一套幫助新主任在關鍵起步期，穩住角色、建立方法、養成節奏、做出成果的增員培訓。
                </p>
                <div className="mt-6 rounded-3xl border border-amber-300/50 bg-amber-300/10 p-5">
                  <p className="text-xl font-black text-amber-100">課程價值</p>
                  <p className="mt-2 text-2xl font-black">穩住角色・建立方法・養成節奏・做出成果</p>
                </div>
              </div>
              <div className="mt-6 rounded-3xl bg-blue-950/60 p-6">
                <p className="text-sm font-semibold text-blue-100/80">測驗結果</p>
                <p className="mt-3 text-xl font-black leading-8 text-white">
                  {showResult && result ? result : "完成左側三題後，點擊按鈕查看建議。"}
                </p>
              </div>
            </CardContent>
          </Card>
        </section>

        <section className="mt-10 rounded-[2rem] border border-amber-300/40 bg-gradient-to-r from-blue-950 via-blue-900 to-orange-900 p-8 text-center shadow-2xl shadow-orange-900/30">
          <p className="text-lg font-bold text-amber-200">主任經典基礎班 × 主任進階班</p>
          <h2 className="mt-2 text-5xl font-black md:text-7xl">從業務高手，到<span className="bg-gradient-to-r from-amber-200 to-orange-400 bg-clip-text text-transparent">增員推手</span></h2>
          <p className="mx-auto mt-5 max-w-3xl text-lg leading-8 text-blue-50/90">邀請你在晉升後的關鍵時刻，打穩增員實戰力。</p>
          <div className="mt-7 flex flex-col justify-center gap-3 sm:flex-row">
            <Button className="rounded-2xl bg-amber-300 px-8 py-6 text-lg font-black text-blue-950 hover:bg-amber-200">我要報名課程</Button>
            <Button variant="outline" className="rounded-2xl border-white/50 bg-white/10 px-8 py-6 text-lg font-black text-white hover:bg-white/20">下載課程介紹</Button>
          </div>
        </section>
      </main>
    </div>
  );
}
