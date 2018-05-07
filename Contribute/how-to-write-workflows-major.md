---
title: Рабочий процесс по внесению значительных или времязатратных изменений на сайте GitHub
description: В этой статье описан рабочий процесс по внесению значительных изменений в статьи на сайте docs.microsoft.com.
author: bryanla
ms.author: bryanla
manager: mbaldwin
ms.date: 08/30/2017
ms.prod: non-product-specific
ms.topic: contributor-guide
ms.custom: external-contributor-guide
ms.openlocfilehash: e26b62923eed22d5b2005b1d84dc4ae240d262b1
ms.sourcegitcommit: dd1b4e915f4996ac029d2a0704ced785438d3484
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2018
---
# <a name="github-contribution-workflow-for-major-or-long-running-changes"></a><span data-ttu-id="d5f6d-103">Рабочий процесс по внесению значительных или времязатратных изменений на сайте GitHub</span><span class="sxs-lookup"><span data-stu-id="d5f6d-103">GitHub contribution workflow for major or long-running changes</span></span>

> [!IMPORTANT]
> <span data-ttu-id="d5f6d-104">При работе со всеми репозиториями, используемыми для публикации на сайте docs.microsoft.com, необходимо соблюдать [правила поведения для управляемых компанией Майкрософт сообществ разработки ПО с открытым кодом](https://opensource.microsoft.com/codeofconduct/) и [правила поведения от .NET Foundation](https://dotnetfoundation.org/code-of-conduct).</span><span class="sxs-lookup"><span data-stu-id="d5f6d-104">All repositories that publish to docs.microsoft.com have adopted either the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/) or the [.NET Foundation Code of Conduct](https://dotnetfoundation.org/code-of-conduct).</span></span> <span data-ttu-id="d5f6d-105">Дополнительные сведения см. на странице с [часто задаваемыми вопросами о правилах поведения](https://opensource.microsoft.com/codeofconduct/faq/).</span><span class="sxs-lookup"><span data-stu-id="d5f6d-105">For more information, see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/).</span></span> <span data-ttu-id="d5f6d-106">С любыми вопросами и комментариями можно также обратиться по адресу [opencode@microsoft.com](mailto:opencode@microsoft.com) или [conduct@dotnetfoundation.org](mailto:conduct@dotnetfoundation.org).</span><span class="sxs-lookup"><span data-stu-id="d5f6d-106">Or contact [opencode@microsoft.com](mailto:opencode@microsoft.com), or [conduct@dotnetfoundation.org](mailto:conduct@dotnetfoundation.org) with any questions or comments.</span></span><br>
>
> <span data-ttu-id="d5f6d-107">Порядок внесения незначительных изменений или уточнений в документацию и примеры кода из общедоступных репозиториев см. в [условиях использования на сайте docs.microsoft.com](https://docs.microsoft.com/legal/termsofuse).</span><span class="sxs-lookup"><span data-stu-id="d5f6d-107">Minor corrections or clarifications to documentation and code examples in public repositories are covered by the [docs.microsoft.com Terms of Use](https://docs.microsoft.com/legal/termsofuse).</span></span> <span data-ttu-id="d5f6d-108">Если новые или значительные изменения вносят не сотрудники корпорации Майкрософт, в комментариях к запросу на вытягивание на сайте GitHub появится предложение принять условия лицензионного соглашения с участником (CLA).</span><span class="sxs-lookup"><span data-stu-id="d5f6d-108">New or significant changes will generate a comment in the pull request, asking you to submit an online Contribution License Agreement (CLA) if you are not an employee of Microsoft.</span></span> <span data-ttu-id="d5f6d-109">Вам нужно заполнить онлайн-форму перед обработкой запроса на вытягивание.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-109">You will need to complete the online form before your pull request can be merged.</span></span>

## <a name="overview"></a><span data-ttu-id="d5f6d-110">Общие сведения</span><span class="sxs-lookup"><span data-stu-id="d5f6d-110">Overview</span></span>

<span data-ttu-id="d5f6d-111">Этот рабочий процесс могут использовать участники, которые вносят значительные или частые изменения в репозиторий.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-111">This workflow is suitable for a contributor who needs to make a major change or will be a frequent contributor to a repository.</span></span> <span data-ttu-id="d5f6d-112">Постоянные участники обычно вносят регулярные или времязатратные изменения, которые предусматривают несколько циклов сборки, проверки и промежуточной обработки или вносятся в течение нескольких дней, прежде чем запрос на вытягивание будет принят и обработан.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-112">Frequent contributors typically have ongoing (long-running) changes, which go through multiple build/validation/staging cycles or span multiple days before pull request sign-off and merge.</span></span>

<span data-ttu-id="d5f6d-113">Ниже представлены примеры таких изменений.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-113">Examples of these types of contributions include:</span></span>

[!INCLUDE[contribute-major-changes-change-definition](includes/contribute-how-to-write-workflows-major-change-definition.md)]

### <a name="terminology"></a><span data-ttu-id="d5f6d-114">Терминология</span><span class="sxs-lookup"><span data-stu-id="d5f6d-114">Terminology</span></span>

<span data-ttu-id="d5f6d-115">Сначала рассмотрим некоторые термины и моникеры Git и GitHub, используемые в этом рабочем процессе.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-115">Before you start, let's review some of the Git/GitHub terms and monikers used in this workflow.</span></span> <span data-ttu-id="d5f6d-116">Вам не обязательно сейчас углубляться в их изучение.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-116">Don't worry about understanding them now.</span></span> <span data-ttu-id="d5f6d-117">Просто ознакомьтесь с терминологией. Вы всегда сможете вернуться к этому разделу, если вам нужно будет что-либо уточнить.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-117">Just know that you will be learning about them, and you can refer back to this section when you need to verify a definition.</span></span>

| <span data-ttu-id="d5f6d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d5f6d-118">Name</span></span> | <span data-ttu-id="d5f6d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d5f6d-119">Description</span></span> |
|-----------|-------------|
|<span data-ttu-id="d5f6d-120">Вилка</span><span class="sxs-lookup"><span data-stu-id="d5f6d-120">fork</span></span>|<span data-ttu-id="d5f6d-121">Этот термин обозначает копию основного репозитория GitHub.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-121">Normally used as a noun, when referring to a copy of a main GitHub repository.</span></span> <span data-ttu-id="d5f6d-122">Фактически вилка — это просто другой репозиторий.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-122">In practice, a fork is just another repository.</span></span> <span data-ttu-id="d5f6d-123">Особенностью вилки является то, что GitHub поддерживает ее подключение к основному (родительскому) репозиторию.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-123">But it's special in the sense that GitHub maintains a connection back to the main/parent repository.</span></span> <span data-ttu-id="d5f6d-124">Иногда этот термин обозначает действие. Например: "Сначала создайте вилку репозитория".</span><span class="sxs-lookup"><span data-stu-id="d5f6d-124">It's sometimes used as a verb, as in "You must fork the repository first."</span></span>|
|<span data-ttu-id="d5f6d-125">Удаленное подключение</span><span class="sxs-lookup"><span data-stu-id="d5f6d-125">remote</span></span>|<span data-ttu-id="d5f6d-126">Именованное подключение к удаленному репозиторию (например, исходному или вышестоящему).</span><span class="sxs-lookup"><span data-stu-id="d5f6d-126">A named connection to a remote repository, such as the "origin" or "upstream" remote.</span></span> <span data-ttu-id="d5f6d-127">В Git такие подключения называются удаленными, так как речь идет о репозитории, размещенном на другом компьютере.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-127">Git refers to these as remotes because they are used to reference a repository that's hosted on another computer.</span></span> <span data-ttu-id="d5f6d-128">В рамках этого рабочего процесса удаленное подключение всегда подразумевает подключение к репозиторию GitHub.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-128">In this workflow, a remote is always a GitHub repository.</span></span>|
|<span data-ttu-id="d5f6d-129">Исходное подключение</span><span class="sxs-lookup"><span data-stu-id="d5f6d-129">origin</span></span>|<span data-ttu-id="d5f6d-130">Это имя подключения между локальным репозиторием и репозиторием, из которого он был клонирован.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-130">The name assigned to the connection between your local repository and the repository from which it was cloned.</span></span> <span data-ttu-id="d5f6d-131">В рамках этого рабочего процесса исходное подключение представляет собой подключение к вилке.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-131">In this workflow, origin represents the connection to your fork.</span></span> <span data-ttu-id="d5f6d-132">Иногда этот термин используется как моникер для самого исходного репозитория. Например: "Не забудьте отправить изменения в исходный репозиторий".</span><span class="sxs-lookup"><span data-stu-id="d5f6d-132">It's sometimes used as a moniker for the origin repository itself, as in "Remember to push your changes to origin."</span></span>|
|<span data-ttu-id="d5f6d-133">Вышестоящее подключение</span><span class="sxs-lookup"><span data-stu-id="d5f6d-133">upstream</span></span>|<span data-ttu-id="d5f6d-134">Как и исходное подключение, вышестоящее подключение — это именованное подключение к другому репозиторию.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-134">Like the origin remote, upstream is a named connection to another repository.</span></span> <span data-ttu-id="d5f6d-135">В рамках этого рабочего процесса вышестоящее подключение представляет собой подключение между локальным и основным репозиторием, из которого создана вилка.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-135">In this workflow, upstream represents the connection between your local repository and the main repository, from which your fork was created.</span></span> <span data-ttu-id="d5f6d-136">Иногда этот термин используется как моникер для самого вышестоящего репозитория. Например: "Не забудьте отправить изменения из вышестоящего репозитория".</span><span class="sxs-lookup"><span data-stu-id="d5f6d-136">It's sometimes used as a moniker for the upstream repository itself, as in "Remember to pull the changes from upstream."</span></span>|

## <a name="workflow"></a><span data-ttu-id="d5f6d-137">Рабочий процесс</span><span class="sxs-lookup"><span data-stu-id="d5f6d-137">Workflow</span></span>

>[!IMPORTANT]
> <span data-ttu-id="d5f6d-138">Если вы еще не сделали это, выполните инструкции из [раздела, посвященного настройке.](get-started-setup-github.md)</span><span class="sxs-lookup"><span data-stu-id="d5f6d-138">If you haven't already, you must complete the steps in the [Setup](get-started-setup-github.md) section.</span></span> <span data-ttu-id="d5f6d-139">Из этого раздела вы узнаете, как настроить учетную запись GitHub, установить Git Bash и Markdown Editor, создать вилку и настроить локальный репозиторий.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-139">This section walks you through setting up your GitHub account, installing Git Bash and a Markdown editor, creating a fork, and setting up your local repository.</span></span> <span data-ttu-id="d5f6d-140">Если вы не работали с Git и GitHub и не знаете, что такое репозиторий или ветвь, сначала ознакомьтесь с [основными понятиями](git-github-fundamentals.md).</span><span class="sxs-lookup"><span data-stu-id="d5f6d-140">If you are unfamiliar with Git and GitHub concepts such as a repository or branch, please first review [Git and GitHub fundamentals](git-github-fundamentals.md).</span></span>

<span data-ttu-id="d5f6d-141">Этот рабочий процесс представляет собой повторяющийся цикл обработки вносимых изменений.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-141">In this workflow, changes flow in a repetitive cycle.</span></span> <span data-ttu-id="d5f6d-142">Сначала вы вносите изменения в локальный репозиторий на вашем устройстве. Затем эти изменения копируются в вашу вилку GitHub, в основной репозиторий GitHub, после чего они снова передаются в локальный репозиторий, когда вы включаете изменения, внесенные другими участниками.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-142">Starting from your device's local repository, they flow back up to your GitHub fork, into the main GitHub repository, and back down locally again as you incorporate changes from other contributors.</span></span>

### <a name="use-github-flow"></a><span data-ttu-id="d5f6d-143">Использование последовательности GitHub</span><span class="sxs-lookup"><span data-stu-id="d5f6d-143">Use GitHub flow</span></span>

<span data-ttu-id="d5f6d-144">Как описано в разделе с [общими сведениями о Git и GitHub](git-github-fundamentals.md#git), репозиторий Git содержит главную ветвь, а также дополнительные ветви в стадии разработки. Эти дополнительные ветви не интегрированы в главную.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-144">Recall from [Git and GitHub fundamentals](git-github-fundamentals.md#git) that a Git repository contains a master branch, plus any additional work-in-progress branches that have not been integrated into master.</span></span> <span data-ttu-id="d5f6d-145">Каждый раз, когда вы вносите логически связанные изменения, лучше всего использовать специально созданную *рабочую ветвь*. Она позволяет управлять изменениями, которые вносятся в рамках этого рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-145">Whenever you introduce a set of logically related changes, it’s a best practice to create a *working branch* to manage your changes through the workflow.</span></span> <span data-ttu-id="d5f6d-146">Эта ветвь называется рабочей, так как она представляет рабочее пространство для итерации и уточнения изменений, которые будут интегрированы обратно в главную ветвь.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-146">We refer to it here as a working branch because it's a workspace to iterate/refine changes, until they can be integrated back into the master branch.</span></span>

<span data-ttu-id="d5f6d-147">Изолируя связанные изменения в конкретной ветви, вы можете самостоятельно отслеживать и внедрять их, назначая им определенное время выпуска в цикле публикации.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-147">Isolating related changes to a specific branch allows you to control and introduce those changes independently, targeting them to a specific release time in the publishing cycle.</span></span> <span data-ttu-id="d5f6d-148">Фактически, работая над определенными задачами, вы можете легко создать несколько рабочих ветвей в своем репозитории.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-148">In reality, depending on the type of work you do, you can easily end up with several working branches in your repository.</span></span> <span data-ttu-id="d5f6d-149">Довольно распространенной практикой является работа сразу в нескольких ветвях, каждая из которых представляет отдельный проект.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-149">It's not uncommon to be working on multiple branches at the same time, each representing a different project.</span></span>

>[!TIP]
><span data-ttu-id="d5f6d-150">*Не рекомендуется* вносить изменения в главную ветвь.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-150">Making your changes in the master branch is *not* a good practice.</span></span> <span data-ttu-id="d5f6d-151">Представим ситуацию, когда вы вносите в главную ветвь блок изменений, выпуск которых запланирован на определенное время.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-151">Imagine that you use the master branch to introduce a set of changes for a timed feature release.</span></span> <span data-ttu-id="d5f6d-152">Изменения внесены, и вы ожидаете их выпуска.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-152">You finish the changes and are waiting to release them.</span></span> <span data-ttu-id="d5f6d-153">В это время вы получаете срочный запрос на исправление. Вы вносите изменения в файл в главной ветви, а затем публикуете это изменение.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-153">Then in the interim, you have an urgent request to fix something, so you make the change to a file in the master branch and then publish the change.</span></span> <span data-ttu-id="d5f6d-154">В итоге получается так, что вы случайно публикуете и исправления, *и* изменения, выпуск которых запланирован на определенную дату.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-154">In this example, you inadvertently publish both the fix *and* the changes that you were holding for release on a specific date.</span></span>

<span data-ttu-id="d5f6d-155">Теперь создадим рабочую ветвь в локальном репозитории, чтобы записать предложенные изменения.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-155">Now let's create a new working branch in your local repository, to capture your proposed changes.</span></span> <span data-ttu-id="d5f6d-156">Клиенты Git отличаются, поэтому ознакомьтесь со справочными сведениями об используемом клиенте.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-156">Each git client is different, so consult the help for your preferred client.</span></span> <span data-ttu-id="d5f6d-157">Дополнительные сведения об этом процессе см. в [соответствующем руководстве GitHub](https://guides.github.com/introduction/flow/).</span><span class="sxs-lookup"><span data-stu-id="d5f6d-157">You can see an overview of the process in the GitHub Guide on [GitHub flow](https://guides.github.com/introduction/flow/).</span></span>

[!INCLUDE[contribute-how-to-write-workflows-pull-request-processing](includes/contribute-how-to-write-workflows-pull-request-processing.md)]

## <a name="next-steps"></a><span data-ttu-id="d5f6d-158">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="d5f6d-158">Next steps</span></span>

<span data-ttu-id="d5f6d-159">Это все!</span><span class="sxs-lookup"><span data-stu-id="d5f6d-159">That's it!</span></span> <span data-ttu-id="d5f6d-160">Вы внесли свой вклад в содержимое сайта docs.microsoft.com.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-160">You've made a contribution to docs.microsoft.com content!</span></span>

- <span data-ttu-id="d5f6d-161">Чтобы узнать больше о разметке Markdown и синтаксисе расширений Markdown, см. раздел с описанием основных средств создания документов.</span><span class="sxs-lookup"><span data-stu-id="d5f6d-161">To learn more about topics such as Markdown and Markdown extensions syntax, continue to the "Writing essentials" section.</span></span>