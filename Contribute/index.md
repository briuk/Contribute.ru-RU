---
title: Руководство для участников разработки документации Майкрософт. Общие сведения
description: В этом руководстве вы узнаете, как создавать статьи для сайта документации Майкрософт docs.microsoft.com.
author: bryanla
ms.author: bryanla
manager: mbaldwin
ms.date: 04/17/2018
ms.prod: non-product-specific
ms.topic: contributor-guide
ms.custom: external-contributor-guide
ms.openlocfilehash: 1cda40c890e5b30e6e1e10f3bcee0278f8004653
ms.sourcegitcommit: 3ec397fab57ea582edb03a59609f62d886410ee8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2018
---
# <a name="microsoft-docs-contributor-guide-overview"></a><span data-ttu-id="a6d54-103">Руководство для участников разработки документации Майкрософт. Общие сведения</span><span class="sxs-lookup"><span data-stu-id="a6d54-103">Microsoft Docs contributor guide overview</span></span>

<span data-ttu-id="a6d54-104">Добро пожаловать в руководство для участников [docs.microsoft.com](https://docs.microsoft.com) (Docs)!</span><span class="sxs-lookup"><span data-stu-id="a6d54-104">Welcome to the [docs.microsoft.com](https://docs.microsoft.com) (Docs) Contributor Guide!</span></span>

<span data-ttu-id="a6d54-105">Некоторая наша документация предоставляется как открытые исходные тексты, размещаемые на портале GitHub.</span><span class="sxs-lookup"><span data-stu-id="a6d54-105">Several of our documentation sets are open source, hosted on GitHub.</span></span> <span data-ttu-id="a6d54-106">Такая модель работы становится все более популярной среди разработчиков.</span><span class="sxs-lookup"><span data-stu-id="a6d54-106">More teams are adopting this model all the time.</span></span> <span data-ttu-id="a6d54-107">Даже документация с частично открытым исходным текстом размещается в общедоступных репозиториях, где вы можете создавать запросы на вытягивание.</span><span class="sxs-lookup"><span data-stu-id="a6d54-107">Even document sets that are not completely open source have public-facing repos where you are invited to make pull requests.</span></span> <span data-ttu-id="a6d54-108">Это упрощает и оптимизирует взаимодействие между разработчиками, отвечающими за содержимое командами и нашими клиентами.</span><span class="sxs-lookup"><span data-stu-id="a6d54-108">It streamlines and improves communication between the product engineers, the content teams, and our customers.</span></span> <span data-ttu-id="a6d54-109">Работа с открытыми исходными текстами дает определенные преимущества.</span><span class="sxs-lookup"><span data-stu-id="a6d54-109">Working in the open provides several advantages:</span></span>

- <span data-ttu-id="a6d54-110">Возможность открытого планирования репозиториев с такими текстами позволяет получать отзывы и комментарии о наиболее востребованной документации.</span><span class="sxs-lookup"><span data-stu-id="a6d54-110">Open source repos plan in the open to get feedback on what docs are most needed.</span></span>
- <span data-ttu-id="a6d54-111">Возможность открытого просмотра репозиториев с такими текстами позволяет публиковать наиболее полезное содержимое при первом выпуске.</span><span class="sxs-lookup"><span data-stu-id="a6d54-111">Open source repos review in the open to publish the most helpful content on our first release.</span></span>
- <span data-ttu-id="a6d54-112">Возможность обновления репозиториев с такими текстами упрощает непрерывный процесс улучшения содержимого.</span><span class="sxs-lookup"><span data-stu-id="a6d54-112">Open source repos update in the open to make it easier to continuously improve the content.</span></span>

<span data-ttu-id="a6d54-113">Пользовательский интерфейс сайта [docs.microsoft.com](https://docs.microsoft.com) непосредственно интегрирует рабочие процессы [GitHub](https://github.com), делая их использование еще более удобными.</span><span class="sxs-lookup"><span data-stu-id="a6d54-113">The user experience on [docs.microsoft.com](https://docs.microsoft.com) integrates [GitHub](https://github.com) workflows directly to make it even easier.</span></span> <span data-ttu-id="a6d54-114">Для начала [отредактируйте просматриваемый документ](#quick-edits-to-existing-documents).</span><span class="sxs-lookup"><span data-stu-id="a6d54-114">Start by [editing the document you are viewing](#quick-edits-to-existing-documents).</span></span> <span data-ttu-id="a6d54-115">Кроме того, вы можете помочь тем, что будете [просматривать новые разделы](#review-open-prs) или [создавать отчеты о проблемах с качеством](#create-quality-issues).</span><span class="sxs-lookup"><span data-stu-id="a6d54-115">Or, help by [reviewing new topics](#review-open-prs), or [create quality issues](#create-quality-issues).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="a6d54-116">При работе со всеми репозиториями, используемыми для публикации на сайте docs.microsoft.com, необходимо соблюдать [правила поведения для управляемых компанией Майкрософт сообществ разработки ПО с открытым кодом](https://opensource.microsoft.com/codeofconduct/) и [правила поведения от .NET Foundation](https://dotnetfoundation.org/code-of-conduct).</span><span class="sxs-lookup"><span data-stu-id="a6d54-116">All repositories that publish to docs.microsoft.com have adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/) or the [.NET Foundation Code of Conduct](https://dotnetfoundation.org/code-of-conduct).</span></span> <span data-ttu-id="a6d54-117">Дополнительные сведения см. на странице с [часто задаваемыми вопросами о правилах поведения](https://opensource.microsoft.com/codeofconduct/faq/).</span><span class="sxs-lookup"><span data-stu-id="a6d54-117">For more information, see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/).</span></span> <span data-ttu-id="a6d54-118">С любыми вопросами и комментариями можно также обратиться по адресу [opencode@microsoft.com](mailto:opencode@microsoft.com) или [conduct@dotnetfoundation.org](mailto:conduct@dotnetfoundation.org).</span><span class="sxs-lookup"><span data-stu-id="a6d54-118">Or contact [opencode@microsoft.com](mailto:opencode@microsoft.com), or [conduct@dotnetfoundation.org](mailto:conduct@dotnetfoundation.org) with any questions or comments.</span></span><br>
>
> <span data-ttu-id="a6d54-119">Порядок внесения незначительных изменений или уточнений в документацию и примеры кода из общедоступных репозиториев см. в [условиях использования на сайте docs.microsoft.com](https://docs.microsoft.com/legal/termsofuse).</span><span class="sxs-lookup"><span data-stu-id="a6d54-119">Minor corrections or clarifications to documentation and code examples in public repositories are covered by the [docs.microsoft.com Terms of Use](https://docs.microsoft.com/legal/termsofuse).</span></span> <span data-ttu-id="a6d54-120">Если новые или значительные изменения вносят не сотрудники корпорации Майкрософт, в комментариях к запросу на вытягивание появляется предложение принять условия лицензионного соглашения с участником (CLA).</span><span class="sxs-lookup"><span data-stu-id="a6d54-120">New or significant changes generate a comment in the pull request, asking you to submit an online Contribution License Agreement (CLA) if you are not an employee of Microsoft.</span></span> <span data-ttu-id="a6d54-121">Вам нужно заполнить онлайн-форму, после чего мы сможем проверить или принять ваш запрос на вытягивание.</span><span class="sxs-lookup"><span data-stu-id="a6d54-121">We need you to complete the online form before we can review or accept your pull request.</span></span>

## <a name="quick-edits-to-existing-documents"></a><span data-ttu-id="a6d54-122">Быстрое редактирование существующей документации</span><span class="sxs-lookup"><span data-stu-id="a6d54-122">Quick edits to existing documents</span></span>

<span data-ttu-id="a6d54-123">Быстрое редактирование позволяет оптимизировать процесс отправки отчетов и устранения небольших ошибок и пропусков в документации.</span><span class="sxs-lookup"><span data-stu-id="a6d54-123">Quick edits streamline the process to report and fix small errors and omissions in documents.</span></span> <span data-ttu-id="a6d54-124">Несмотря на все прилагаемые усилия, в публикуемых документах все же встречаются несущественные грамматические ошибки и опечатки.</span><span class="sxs-lookup"><span data-stu-id="a6d54-124">Despite all efforts, small grammar and spelling errors do make their way into our published documents.</span></span> <span data-ttu-id="a6d54-125">Вы можете создавать отчеты об ошибках, но быстрее и проще создать запрос на вытягивание, чтобы исправить ошибку.</span><span class="sxs-lookup"><span data-stu-id="a6d54-125">While you can create issues to report mistakes, it's faster and easier to create a pull request (PR) to fix the issue.</span></span> <span data-ttu-id="a6d54-126">Практически в каждой статье есть кнопка редактирования, как показано на следующем рисунке.</span><span class="sxs-lookup"><span data-stu-id="a6d54-126">Almost every article displays an edit button as shown in the following figure.</span></span> <span data-ttu-id="a6d54-127">После нажатия кнопки **Изменить** откроется исходный файл, размещенный на сайте GitHub.</span><span class="sxs-lookup"><span data-stu-id="a6d54-127">Clicking the **Edit** button takes you to the source file on GitHub.</span></span>

![Расположение ссылки "Изменить"](./media/index/edit-article.png)

<span data-ttu-id="a6d54-129">После этого щелкните значок карандаша, показанный на следующем рисунке, чтобы отредактировать статью.</span><span class="sxs-lookup"><span data-stu-id="a6d54-129">Next, click the pencil icon, shown in the following figure to edit the article.</span></span>

> [!NOTE]
> <span data-ttu-id="a6d54-130">Если значок карандаша неактивен, необходимо войти в существующую учетную запись на сайте GitHub или создать новую.</span><span class="sxs-lookup"><span data-stu-id="a6d54-130">If the pencil icon is grayed out, you need to login to your GitHub account, or create a new account.</span></span> <span data-ttu-id="a6d54-131">Внесите необходимые изменения в веб-редакторе.</span><span class="sxs-lookup"><span data-stu-id="a6d54-131">Make your changes in the web editor.</span></span> <span data-ttu-id="a6d54-132">Можно щелкнуть вкладку **Preview changes** (Предварительный просмотр изменений), чтобы проверить форматирование измененного текста.</span><span class="sxs-lookup"><span data-stu-id="a6d54-132">You can click the **Preview changes** tab to check formatting of your change.</span></span>

![Расположение значка карандаша](./media/index/editicon.png)

<span data-ttu-id="a6d54-134">Закончив вносить изменения, прокрутите страницу вниз до конца.</span><span class="sxs-lookup"><span data-stu-id="a6d54-134">Once you have made your changes, scroll to the bottom of the page.</span></span> <span data-ttu-id="a6d54-135">Введите заголовок и описание вашего запроса на вытягивание и нажмите кнопку **Propose file change** (Предложить изменение файла), как показано на рисунке ниже:</span><span class="sxs-lookup"><span data-stu-id="a6d54-135">Enter a title and description for your PR and click **Propose file change** as shown in the following figure:</span></span>

![Предложение изменения](./media/index/submit-pull-request.png)

<span data-ttu-id="a6d54-137">Это все!</span><span class="sxs-lookup"><span data-stu-id="a6d54-137">That's it!</span></span> <span data-ttu-id="a6d54-138">Участники команды по созданию содержимого проверят ваш запрос на вытягивание и выполнят слияние.</span><span class="sxs-lookup"><span data-stu-id="a6d54-138">Content team members will review and merge your PR.</span></span> <span data-ttu-id="a6d54-139">Вы можете получить ответ с просьбой отредактировать изменения, если вы внесли значительные правки.</span><span class="sxs-lookup"><span data-stu-id="a6d54-139">You may get some feedback requesting changes if you made larger changes.</span></span>

<span data-ttu-id="a6d54-140">Пользовательский интерфейс редактирования сайта GitHub может реагировать по-разному в зависимости от ваших разрешений на работу с репозиторием.</span><span class="sxs-lookup"><span data-stu-id="a6d54-140">The GitHub editing UI responds to your permissions on the repository.</span></span> <span data-ttu-id="a6d54-141">Предыдущие рисунки актуальны для участников, которые не имеют разрешения на запись в целевом репозитории.</span><span class="sxs-lookup"><span data-stu-id="a6d54-141">The preceding images are accurate for contributors that do not have write permissions to the target repository.</span></span> <span data-ttu-id="a6d54-142">GitHub автоматически создает вилку целевого репозитория в вашей учетной записи.</span><span class="sxs-lookup"><span data-stu-id="a6d54-142">GitHub automatically creates a fork of the target repository in your account.</span></span> <span data-ttu-id="a6d54-143">Если у вас есть доступ на запись в целевом репозитории, GitHub создает в нем новую ветвь.</span><span class="sxs-lookup"><span data-stu-id="a6d54-143">If you have write access to the target repository, GitHub creates a new branch in the target repo.</span></span> <span data-ttu-id="a6d54-144">Имя ветви указано в формате **\<GitHubId\>-patch-n**, где GitHubId — ваш идентификатор на сайте GitHub, а patch-n — числовой идентификатор исправления.</span><span class="sxs-lookup"><span data-stu-id="a6d54-144">The branch name has the form **\<GitHubId\>-patch-n** using your GitHub ID, and a numeric identifier for the patch branch.</span></span>

<span data-ttu-id="a6d54-145">Запросы на вытягивание используются для всех изменений, даже если участники имеют доступ для записи.</span><span class="sxs-lookup"><span data-stu-id="a6d54-145">We use PRs for all changes, even for contributors that have write access.</span></span> <span data-ttu-id="a6d54-146">В большинстве репозиториев ветвь `master` защищена, так что обновления должны отправляться в виде запросов на вытягивание.</span><span class="sxs-lookup"><span data-stu-id="a6d54-146">Most repositories have the `master` branch protected so that updates must be submitted as PRs.</span></span>

<span data-ttu-id="a6d54-147">Редактирование в браузере лучше использовать для незначительных и эпизодических изменений.</span><span class="sxs-lookup"><span data-stu-id="a6d54-147">The in-browser editing experience is best for minor or infrequent changes.</span></span> <span data-ttu-id="a6d54-148">Если вы вносите значительные изменения или используете расширенные возможности Git (например, управление ветвлением или дополнительные варианты устранения конфликтов при слиянии), вам необходимо [создать вилку репозитория и работать локально](how-to-write-workflows-major.md).</span><span class="sxs-lookup"><span data-stu-id="a6d54-148">If you make large contributions, or use advanced Git features (such as branch management or advanced merge conflict resolution), you need to [fork the repo and work locally](how-to-write-workflows-major.md).</span></span>

## <a name="review-open-prs"></a><span data-ttu-id="a6d54-149">Проверка открытых запросов на вытягивание</span><span class="sxs-lookup"><span data-stu-id="a6d54-149">Review open PRs</span></span>

<span data-ttu-id="a6d54-150">Вы можете просматривать новые разделы до их публикации, проверяя открытые запросы на вытягивание.</span><span class="sxs-lookup"><span data-stu-id="a6d54-150">You can read new topics before they are published by checking the currently open PRs.</span></span> <span data-ttu-id="a6d54-151">Проверки выполняются в соответствии с процедурой [последовательности GitHub](https://guides.github.com/introduction/flow/).</span><span class="sxs-lookup"><span data-stu-id="a6d54-151">Reviews follow the [GitHub flow](https://guides.github.com/introduction/flow/) process.</span></span> <span data-ttu-id="a6d54-152">Предложенные обновления и новые статьи можно увидеть в общедоступных репозиториях.</span><span class="sxs-lookup"><span data-stu-id="a6d54-152">You can see proposed updates or new articles in public repositories.</span></span> <span data-ttu-id="a6d54-153">Вы можете проверять их и добавлять комментарии.</span><span class="sxs-lookup"><span data-stu-id="a6d54-153">Review them and add your comments.</span></span> <span data-ttu-id="a6d54-154">Просматривайте любые наши репозитории с документацией и открытые запросы на вытягивание с интересующей вас тематикой.</span><span class="sxs-lookup"><span data-stu-id="a6d54-154">Look at any of our docs repositories, and check the open pull requests (PRs) for areas that interest you.</span></span> <span data-ttu-id="a6d54-155">Отзывы пользователей о предлагаемых обновлениях идут на пользу всему сообществу.</span><span class="sxs-lookup"><span data-stu-id="a6d54-155">Community feedback on proposed updates helps the entire community.</span></span>

## <a name="create-quality-issues"></a><span data-ttu-id="a6d54-156">Создание отчетов о проблемах с качеством</span><span class="sxs-lookup"><span data-stu-id="a6d54-156">Create quality issues</span></span>

<span data-ttu-id="a6d54-157">Мы постоянно работаем над улучшением нашей документации.</span><span class="sxs-lookup"><span data-stu-id="a6d54-157">Our docs are a continuous work in progress.</span></span> <span data-ttu-id="a6d54-158">Качественные запросы помогают нам сосредоточиться на наиболее приоритетных для сообщества направлениях.</span><span class="sxs-lookup"><span data-stu-id="a6d54-158">Good issues help us focus our efforts on the highest priorities for the community.</span></span> <span data-ttu-id="a6d54-159">Чем больше информации мы получаем от вас, тем полезнее ваш запрос.</span><span class="sxs-lookup"><span data-stu-id="a6d54-159">The more detail you can provide, the more helpful the issue.</span></span> <span data-ttu-id="a6d54-160">Расскажите нам о том, какую информацию вы искали.</span><span class="sxs-lookup"><span data-stu-id="a6d54-160">Tell us what information you sought.</span></span> <span data-ttu-id="a6d54-161">Расскажите о том, какие условия поиска вы использовали.</span><span class="sxs-lookup"><span data-stu-id="a6d54-161">Tell us the search terms you used.</span></span> <span data-ttu-id="a6d54-162">Если вы не знаете, с чего начать, расскажите о том, с чего вы хотели бы начать знакомство с новой технологией.</span><span class="sxs-lookup"><span data-stu-id="a6d54-162">If you can't get started, tell us how you want to start exploring unfamiliar technology.</span></span>

<span data-ttu-id="a6d54-163">Чтобы понять ваши потребности, нам необходимы ваши отзывы.</span><span class="sxs-lookup"><span data-stu-id="a6d54-163">Issues start the conversation about what's needed.</span></span> <span data-ttu-id="a6d54-164">Команда по созданию содержимого ответит на эти запросы, предложив возможные варианты решения, и поинтересуется вашим мнением.</span><span class="sxs-lookup"><span data-stu-id="a6d54-164">The content team will respond to these issues with ideas for what we can add, and ask for your opinions.</span></span> <span data-ttu-id="a6d54-165">Когда проект решения будет готов, мы попросим вас [проверить запрос на вытягивание](#review-open-prs).</span><span class="sxs-lookup"><span data-stu-id="a6d54-165">When we create a draft, we'll ask you to [review the PR](#review-open-prs).</span></span>

## <a name="get-more-involved"></a><span data-ttu-id="a6d54-166">Узнайте больше</span><span class="sxs-lookup"><span data-stu-id="a6d54-166">Get more involved</span></span>

<span data-ttu-id="a6d54-167">В других разделах представлена информация, которая поможет вам стать участником и внести свой вклад в развитие документации Майкрософт. В них разъясняются принципы работы с репозиториями GitHub, средствами Markdown и расширениями, используемыми на платформе документации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="a6d54-167">Other topics help you get started productively contributing to Microsoft Docs. They explain working with GitHub repositories, Markdown tools, and extensions used in the Microsoft Docs platform.</span></span>