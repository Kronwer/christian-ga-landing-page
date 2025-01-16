<template>
    <UCard>
        <div class="mb-3">
            <p class="font-semibold text-lg lg:text-xl xl:text-2xl">Experience</p>
        </div>
        <div class="flex flex-col gap-3">
            <ItemExperience
                imageUrl="mindden_logo.jpg"
                companyName="MindDen"
                title=".NET Software Developer"
                period="jan. 2025 - current"
                technologies=".NET, SQL Server, RabbitMQ, SignalR, Entity Framework Core"
            />
            <ItemExperience
                imageUrl="unit4_logo.jpg"
                companyName="Unit4"
                title="Associate Software Engineer"
                period="abr. 2023 - jan. 2025"
                technologies=".NET, Azure Cloud, SQL Server"
            />
            <ItemExperience
                imageUrl="unit4_logo.jpg"
                companyName="Unit4"
                title="Software Engineer Intern"
                period="dic. 2022 - mar. 2023"
                technologies="React, .NET, Azure Cloud, SQL Server"
            />
            <ItemExperience
                imageUrl="biit_logo.jpg"
                companyName="BiiT Sourcing Solutions"
                title="Full Stack Developer Intern"
                period="feb. 2022 - jul. 2022"
                technologies="Angular, TypeScript, Java Spring, SQL Server"
            />
        </div>
    </UCard>
</template>