# the_theory_of_function_of_complex_variable

\documentclass[12pt]{article}
\usepackage{amsmath,amssymb}
\usepackage{graphicx}
\usepackage{placeins}
\usepackage[T2A]{fontenc}
\usepackage[utf8]{inputenc}
\usepackage[russian]{babel}

\title{Теория функций комплексной переменной. ИДЗ 1}
\author{Гузовская Александра Чеславовна, Б9123-01.03.02сп}
\date{27 марта 2025}

\begin{document}

\section{Найти все значения корня $\sqrt[3]{i}$}
корень некоторой степени из комплексного числа находится по формуле
$$\sqrt[n]{z} = \sqrt[n]{r}\bigg(\cos{\frac{\varphi+2\pi k}{n}}+ \sin{\frac{\varphi+2\pi k}{n}}\bigg)$$
где r есть модуль комплексного числа z, k изменяется от 0 до n-1, всего n значений корня комплексного числа n-ой степени
$$z_k = \sqrt[n]{r}\bigg(\cos{\frac{\varphi+2\pi k}{n}} + \sin{\frac{\varphi+2\pi k}{n}}\bigg)$$
подставляя значения k постепенно получим все корни\\
рассмотрим данный случай из задания: модуль этого комплексного числа равен 1, степень искомая равня трём, подставим\\
$$z_0 = \sqrt[3]{1}\bigg(\cos{\frac{\varphi+2\pi \cdot 0}{3}}+ i\sin{\frac{\varphi+2\pi \cdot 0}{3}}\bigg) = \cos{\frac{\varphi}{3}} + \sin{\frac{\varphi}{3}}$$
$$z_1 = \sqrt[3]{1}\bigg(\cos{\frac{\varphi+2\pi \cdot 1}{3}}+ i\sin{\frac{\varphi+2\pi \cdot 1}{3}}\bigg) = \cos{\frac{\varphi + 2\pi}{3}} + i\sin{\frac{\varphi + 2\pi}{3}}$$
$$z_2 = \sqrt[3]{1}\bigg(\cos{\frac{\varphi+2\pi \cdot 2}{3}}+ i\sin{\frac{\varphi+2\pi \cdot 2}{3}}\bigg) = \cos{\frac{\varphi + 4\pi}{3}} + i\sin{\frac{\varphi + 4\pi}{3}}$$
из алгебраического представления комплексного числа мы также можем узнать его аргумент (угол $\varphi = \arctan{\frac{b}{a}}$), в нашем случае a = b = 1, $\arctan{1} = \frac{\pi}{4}$\\
$$\cos{\frac{\pi}{12}} + \sin{\frac{\pi}{12}}$$
$$\cos{\frac{9\pi}{12}} + i\sin{\frac{9\pi}{12}} = \cos{\frac{3\pi}{4}} + i\sin{\frac{3\pi}{4}}$$
$$\cos{\frac{17\pi}{12}} + \sin{\frac{17\pi}{12}}$$
Получим ответ: $\sqrt[3]{i} = \{ \frac{\sqrt{3}}{2} + i\frac{1}{2}; -\frac{\sqrt{3}}{2} + i\frac{1}{2}; -i \}$
\section{Представить в алгебраической форме}
\subsection{ $\cos{(\frac{\pi}{6} - i)}$}
Используем формулу косинуса разности\\
$$\cos{\frac{\pi}{6} - i} = \cos{\frac{\pi}{6}} \cdot \cos{i} + \sin{\frac{\pi}{6}} \cdot \sin{i}$$
Функции с мнимыми аргументами представим в виде показательных:\\
$$\frac{\sqrt{3}}{2} \cdot \frac{e^{-1} + e^1}{2} + \frac{1}{2} \cdot \frac{e^{-1} - e^1}{2i} = \bigg(\frac{\sqrt{3}}{2} \cdot \frac{e^{-1} + e^1}{2} \bigg) + i \cdot \bigg(\frac{1}{2} \cdot \frac{e^1 - e^{-1}}{2}\bigg)$$
это же и оставляется как ответ:
$$\bigg(\frac{\sqrt{3} \cdot (e^{-1} + e^1)}{4} \bigg) + i \cdot \bigg(\frac{e^1 - e^{-1}}{4} \bigg)$$

\subsection{$arth \bigg(\frac{3 + i\cdot2\sqrt{3}}{7}\bigg)$}
Перейдём от гиперболической функции к арктангенсу тригонометрическому, а после к выражению его через натуральный логарифм\\
$$arth(z) = i \cdot arctg(\frac{z}{i}) = i \cdot \bigg(-\frac{i}{2} \cdot Ln\Big( \frac{1+i\cdot \frac{z}{i}}{1 - i\cdot \frac{z}{i}}\Big)\bigg) = \frac{1}{2} \cdot Ln \Big(\frac{1+z}{1-z}\Big)$$
подставим значение z из условия: $z = \frac{3 + i \cdot 2\sqrt{3}}{3}$
$$arth\bigg(\frac{3+i\cdot 2\sqrt{3}}{3}\bigg) = \frac{1}{2} \cdot Ln \bigg(\frac{1 + \frac{3 + i\cdot 2\sqrt{3}}{3}}{1 - \frac{3 + i\cdot 2\sqrt{3}}{3}} \bigg) = \frac{1}{2} \cdot Ln\bigg(\frac{6 + i\cdot2\sqrt{3}}{-i\cdot 2\sqrt{3}}\bigg) = $$
$$= \frac{1}{2}\cdot Ln\bigg(\frac{\sqrt{3} + i}{-i} \bigg) = \frac{1}{2}\cdot Ln(i\sqrt{3} - 1)$$
Логарифмическая функция Ln(z), $z \neq 0$ определяется как обратная показательной и имеет вид: $Ln(z) = ln|z| + i\cdot Arg(z) = ln|z| + i(arg(z) + 2\pi k), k = 0, \pm 1, \pm 2, ...$
подставим это в ранее полученное $\frac{1}{2}\cdot Ln(i\sqrt{3} - 1)$\\
$$\frac{1}{2}\cdot Ln(i\sqrt{3} - 1) = \frac{1}{2}\cdot \bigg(ln|i\sqrt{3} - 1| + i\cdot \Big(arg(i\sqrt{3} - 1) + 2\pi k\Big) \bigg) =$$
$$\frac{1}{2}\cdot ln(2) + \frac{i}{2}\bigg(arg(i\sqrt{3} - 1) +2\pi k\bigg) \approx \frac{1}{2} \cdot 0,693 + \frac{i}{2}(\frac{2\pi}{3} + 2\pi k), k = 0, \pm 1, \pm 2, ...$$

\subsection{$(-1 + 2i)^{2i}$}
rgdrdfgt
\subsection{$Ln(1+i)$}
Логарифмическая функция Ln(z), $z \neq 0$ определяется как обратная показательной и имеет вид: $$Ln(z) = ln|z| + i\cdot Arg(z) = ln|z| + i(arg(z) + 2\pi k), k = 0, \pm 1, \pm 2, ...$$
подставим значение комплексного числа из задания\\
 $$Ln(1+i) = ln|1+i| + i\cdot Arg(1+i) = ln \sqrt{2} + i(arg(1+i) + 2\pi k) \approx$$ $$\approx 0,347 + i(\frac{\pi}{4} + 2\pi k), k = 0, \pm 1, \pm 2, ...$$

\section{Вычертить область, заданную неравенствами:}
\section{Определить вид пути в случае, когда он проходит через точку $\infty$, исследовать его поведение в этой точке:}
\section{Восстановить голоморфную в окрестности точки $z_0$ функцию $f(z)$ по известной действительной части $u(x,y)$ или мнимой $v(x,y)$ и начальному значению $f(z_o): v = x^2 - y^2 + 2x + 1, f(0) = i.$}
\section{Introduction}
\section{Introduction}

\end{document}
