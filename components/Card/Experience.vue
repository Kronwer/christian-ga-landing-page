<template>
    <UCard>
        <div class="mb-3">
            <p class="font-semibold text-lg">Experience</p>
        </div>
        <div class="flex flex-col gap-3">
            <ItemExperience
                imageUrl="unit4_logo.jpg"
                companyName="Unit4"
                title="Associate Software Engineer"
                period="abr. 2023 - current"
                technologies=".NET, SQL Server, Azure Cloud"
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
                title="Frontend Developer Intern"
                period="feb. 2022 - jul. 2022"
                technologies="Angular, TypeScript, Java Spring, SQL Server"
            />
        </div>
    </UCard>
</template>