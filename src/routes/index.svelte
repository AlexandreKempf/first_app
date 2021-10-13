<script>
import TextInput from './TextInput.svelte';
import DateInput from './DateInput.svelte';
import RadioInput from './RadioInput.svelte';
import SelectInput from './SelectInput.svelte';
</script>

<link rel="stylesheet" href="https://rsms.me/inter/inter.css">


<div class="lg:grid lg:grid-cols-12 lg:gap-x-5">
  <aside class="py-6 px-2 sm:px-6 lg:py-0 lg:px-0 lg:col-span-3">
    <nav class="space-y-1">
      <!-- Current: "bg-gray-50 text-indigo-700 hover:text-indigo-700 hover:bg-white", Default: "text-gray-900 hover:text-gray-900 hover:bg-gray-50" -->
      <a href="#Identification" class="bg-gray-50 text-indigo-700 hover:text-indigo-700 hover:bg-white group rounded-md px-3 py-2 flex items-center text-sm font-medium" aria-current="page">
        <!--
          Heroicon name: outline/user-circle

          Current: "text-indigo-500 group-hover:text-indigo-500", Default: "text-gray-400 group-hover:text-gray-500"
        -->
        <svg class="text-indigo-500 group-hover:text-indigo-500 flex-shrink-0 -ml-1 mr-3 h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5.121 17.804A13.937 13.937 0 0112 16c2.5 0 4.847.655 6.879 1.804M15 10a3 3 0 11-6 0 3 3 0 016 0zm6 2a9 9 0 11-18 0 9 9 0 0118 0z" />
        </svg>
        <span class="truncate">
          Identification
        </span>
      </a>

      <a href="#HistoireFamiliale" class="text-gray-900 hover:text-gray-900 hover:bg-gray-50 group rounded-md px-3 py-2 flex items-center text-sm font-medium">
				<svg class="text-gray-400 group-hover:text-gray-500 flex-shrink-0 -ml-1 mr-3 h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 20h5v-2a3 3 0 00-5.356-1.857M17 20H7m10 0v-2c0-.656-.126-1.283-.356-1.857M7 20H2v-2a3 3 0 015.356-1.857M7 20v-2c0-.656.126-1.283.356-1.857m0 0a5.002 5.002 0 019.288 0M15 7a3 3 0 11-6 0 3 3 0 016 0zm6 3a2 2 0 11-4 0 2 2 0 014 0zM7 10a2 2 0 11-4 0 2 2 0 014 0z" />
        </svg>
        <span class="truncate">
          Histoire familiale
        </span>
      </a>

      <a href="#HistoireGrossesse" class="text-gray-900 hover:text-gray-900 hover:bg-gray-50 group rounded-md px-3 py-2 flex items-center text-sm font-medium">
        <svg class="text-gray-400 group-hover:text-gray-500 flex-shrink-0 -ml-1 mr-3 h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
  				<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10 6H5a2 2 0 00-2 2v9a2 2 0 002 2h14a2 2 0 002-2V8a2 2 0 00-2-2h-5m-4 0V5a2 2 0 114 0v1m-4 0a2 2 0 104 0m-5 8a2 2 0 100-4 2 2 0 000 4zm0 0c1.306 0 2.417.835 2.83 2M9 14a3.001 3.001 0 00-2.83 2M15 11h3m-3 4h2" />
        </svg>
        <span class="truncate">
          Histoire de la grossesse et de la naissance
        </span>
      </a>

      <a href="#HistoireMedicale" class="text-gray-900 hover:text-gray-900 hover:bg-gray-50 group rounded-md px-3 py-2 flex items-center text-sm font-medium">
        <svg class="text-gray-400 group-hover:text-gray-500 flex-shrink-0 -ml-1 mr-3 h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
				  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 9v3m0 0v3m0-3h3m-3 0H9m12 0a9 9 0 11-18 0 9 9 0 0118 0z" />
        </svg>
        <span class="truncate">
          Histoire médicale
        </span>
      </a>

      <a href="#HistoireDeveloppement" class="text-gray-900 hover:text-gray-900 hover:bg-gray-50 group rounded-md px-3 py-2 flex items-center text-sm font-medium">
        <svg class="text-gray-400 group-hover:text-gray-500 flex-shrink-0 -ml-1 mr-3 h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
				  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M11 4a2 2 0 114 0v1a1 1 0 001 1h3a1 1 0 011 1v3a1 1 0 01-1 1h-1a2 2 0 100 4h1a1 1 0 011 1v3a1 1 0 01-1 1h-3a1 1 0 01-1-1v-1a2 2 0 10-4 0v1a1 1 0 01-1 1H7a1 1 0 01-1-1v-3a1 1 0 00-1-1H4a2 2 0 110-4h1a1 1 0 001-1V7a1 1 0 011-1h3a1 1 0 001-1V4z" />
				</svg>
        <span class="truncate">
          Histoire du développement
        </span>
      </a>

			<a href="#HistoireScolaire" class="text-gray-900 hover:text-gray-900 hover:bg-gray-50 group rounded-md px-3 py-2 flex items-center text-sm font-medium">
				<svg class="text-gray-400 group-hover:text-gray-500 flex-shrink-0 -ml-1 mr-3 h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
				  <path d="M12 14l9-5-9-5-9 5 9 5z" />
				  <path d="M12 14l6.16-3.422a12.083 12.083 0 01.665 6.479A11.952 11.952 0 0012 20.055a11.952 11.952 0 00-6.824-2.998 12.078 12.078 0 01.665-6.479L12 14z" />
				<path strokeLinecap="round" strokeLinejoin="round" strokeWidth={2} d="M12 14l9-5-9-5-9 5 9 5zm0 0l6.16-3.422a12.083 12.083 0 01.665 6.479A11.952 11.952 0 0012 20.055a11.952 11.952 0 00-6.824-2.998 12.078 12.078 0 01.665-6.479L12 14zm-4 6v-7.5l4-2.222" />
				</svg>
        <span class="truncate">
					Histoire scolaire
        </span>
      </a>

			<a href="#ElementsComplementaires" class="text-gray-900 hover:text-gray-900 hover:bg-gray-50 group rounded-md px-3 py-2 flex items-center text-sm font-medium">
				<svg class="text-gray-400 group-hover:text-gray-500 flex-shrink-0 -ml-1 mr-3 h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
					<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 14v6m-3-3h6M6 10h2a2 2 0 002-2V6a2 2 0 00-2-2H6a2 2 0 00-2 2v2a2 2 0 002 2zm10 0h2a2 2 0 002-2V6a2 2 0 00-2-2h-2a2 2 0 00-2 2v2a2 2 0 002 2zM6 20h2a2 2 0 002-2v-2a2 2 0 00-2-2H6a2 2 0 00-2 2v2a2 2 0 002 2z" />
				</svg>
				<span class="truncate">
					Eléments complémentaires
				</span>
			</a>

    </nav>
  </aside>

  <div class="space-y-6 sm:px-6 lg:px-0 lg:col-span-9">
    <form action="#" method="POST">
      <div class="shadow sm:rounded-md sm:overflow-hidden bg-white py-6 px-4 space-y-6 sm:p-6">
          <div>
            <h3 id="Identification">Identification</h3>
            <p class="mt-1 text-sm text-gray-500">Informations concernant votre enfant.</p>
          </div>

          <div class="grid grid-cols-12 gap-12">
						<div class="col-span-12 sm:col-span-6 lg:col-span-4"><TextInput name="first_name" label="Prénom"/></div>
            <div class="col-span-12 sm:col-span-6 lg:col-span-4"><TextInput name="last_name" label="Nom"/></div>
						<div class="col-span-12 sm:col-span-6 lg:col-span-4"><DateInput name="birth_date" label="Date de naissance"/></div>

						<div class="col-span-12 sm:col-span-6 lg:col-span-3">
              <RadioInput name="dominant_hand" options={["Droitier", "Gaucher", "Ambidextre"]} />
					  </div>
            <div class="col-span-12 sm:col-span-6 lg:col-span-3"><TextInput name="school_grade" label="Scolarisé en" placeholder="CE1"/></div>
            <div class="col-span-12 sm:col-span-6 lg:col-span-3"><TextInput name="teacher_name" label="Nom de l’enseignant"/></div>
            <div class="col-span-12 sm:col-span-6 lg:col-span-3"><TextInput name="school_name" label="École"/></div>
					</div>
      </div>
		</form>

    <form action="#" method="POST">
      <div class="shadow sm:rounded-md sm:overflow-hidden bg-white py-6 px-4 space-y-6 sm:p-6">
          <div>
            <h3 id="HistoireFamiliale">Histoire Familiale</h3>
            <p class="mt-1 text-sm text-gray-500">Informations concernant la famille de l'enfant.</p>
          </div>

					<legend class="text-base font-medium text-gray-900">Mère de l'enfant</legend>
          <div class="grid grid-cols-12 gap-12">
            <div class="col-span-12 sm:col-span-6 lg:col-span-4"><TextInput name="mother_first_name" label="Prénom"/></div>
            <div class="col-span-12 sm:col-span-6 lg:col-span-4"><TextInput name="mother_last_name" label="Nom"/></div>
            <div class="col-span-12 sm:col-span-6 lg:col-span-4"><DateInput name="mother_birth_date" label="Date de naissance"/></div>

            <div class="col-span-12 sm:col-span-6 lg:col-span-6"><TextInput name="mother_job" label="Profession"/></div>
            <div class="col-span-12 sm:col-span-6 lg:col-span-6"><TextInput name="mother_adress" label="Adresse du domicile"/></div>

            <div class="col-span-12 sm:col-span-4 lg:col-span-3"><TextInput name="mother_email" label="Adresse mail" placeholder="you@gmail.com"/></div>
            <div class="col-span-12 sm:col-span-4 lg:col-span-3"><TextInput name="mother_phone_1" label="Mobile"/></div>
            <div class="col-span-12 sm:col-span-4 lg:col-span-3"><TextInput name="mother_phone_2" label="Téléphone fixe"/></div>
					</div>

					<div class="relative absolute inset-0 flex items-center w-full border-t border-gray-300" aria-hidden="true"></div>

					<legend class="pt-6 text-base font-medium text-gray-900">Père de l'enfant</legend>
          <div class="grid grid-cols-12 gap-12">
            <div class="col-span-12 sm:col-span-6 lg:col-span-4"><TextInput name="father_first_name" label="Prénom"/></div>
            <div class="col-span-12 sm:col-span-6 lg:col-span-4"><TextInput name="father_last_name" label="Nom"/></div>
            <div class="col-span-12 sm:col-span-6 lg:col-span-4"><DateInput name="father_birth_date" label="Date de naissance"/></div>

            <div class="col-span-12 sm:col-span-6 lg:col-span-6"><TextInput name="father_job" label="Profession"/></div>
            <div class="col-span-12 sm:col-span-6 lg:col-span-6"><TextInput name="father_adress" label="Adresse du domicile"/></div>


            <div class="col-span-12 sm:col-span-4 lg:col-span-3"><TextInput name="father_email" label="Adresse mail" placeholder="you@gmail.com"/></div>
            <div class="col-span-12 sm:col-span-4 lg:col-span-3"><TextInput name="father_phone_1" label="Mobile"/></div>
            <div class="col-span-12 sm:col-span-4 lg:col-span-3"><TextInput name="father_phone_2" label="Téléphone fixe"/></div>
          </div>

          <div class="relative absolute inset-0 flex items-center w-full border-t border-gray-300" aria-hidden="true"></div>

          <legend class="pt-6 text-base font-medium text-gray-900">Situation des parents</legend>
          <div class="grid grid-cols-12 gap-12">
            <div class="col-span-12 sm:col-span-3">
              <SelectInput name="parents_situation" label="Les parents sont" options={["mariés", "en vie commune", "divorcés", "séparés", "décédés"]} />
            </div>
            <div class="col-span-12 sm:col-span-6 lg:col-span-3"><DateInput name="parents_situation_date" label="Depuis le"/></div>

            <div class="col-span-12 sm:col-span-3">
              <SelectInput name="parents_garde" label="L'enfant vit principalement avec" options={["les deux parents", "sa mère", "son père", "une garde alternée équitable", "famille d'acceuil", "autre"]} />
            </div>
            <div class="col-span-12 sm:col-span-6 lg:col-span-3"><DateInput name="parents_situation_date" label="Depuis le"/></div>

            <div class="col-span-12 sm:col-span-6 lg:col-span-3">
              <RadioInput name="adoption_bool" label="L'enfant a t'il été adopté" options={["Oui", "Non"]} />
					  </div>
            <div class="col-span-12 sm:col-span-6 lg:col-span-3">
              <TextInput name="adoption_age" label="Si oui, à quel age ?"/>
					  </div>
          </div>

          <div class="relative absolute inset-0 flex items-center w-full border-t border-gray-300" aria-hidden="true"></div>

          <legend class="pt-6 text-base font-medium text-gray-900">Fratrie</legend>


          </div>
		</form>
  </div>
</div>



<style global lang="postcss">
  @tailwind base;
  @tailwind components;
  @tailwind utilities;

	@layer base {
	  	h3 {@apply text-lg leading-6 font-medium text-gray-900}
	}
</style>
