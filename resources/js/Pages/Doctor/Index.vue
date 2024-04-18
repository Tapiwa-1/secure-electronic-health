<script setup>
import AuthenticatedLayout from '@/Layouts/AuthenticatedLayout.vue';
import { Head,Link } from '@inertiajs/vue3';
</script>

<template>
    <Head title="Doctors" />

    <AuthenticatedLayout>
        <template #header>
            <h2 class="font-semibold text-xl text-gray-800 leading-tight">Doctors Here</h2>
        </template>

        <div class="py-12">
            <div class="max-w-7xl mx-auto my-4 sm:px-6 lg:px-8">
                 <Link type="button" role="button" :href="route('admin.doctor.create')" class="text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5 me-2 mb-2 dark:bg-blue-600 dark:hover:bg-blue-700 focus:outline-none dark:focus:ring-blue-800">Add Doctor</Link>
            </div>

            <div class="max-w-7xl mx-auto sm:px-6 lg:px-8">

                <div class="bg-white overflow-hidden shadow-sm sm:rounded-lg">

                <div class="relative overflow-x-auto">
                    <table class="w-full text-sm text-left rtl:text-right text-gray-500 ">
                        <thead class="text-xs text-gray-700 uppercase bg-gray-50">
                            <tr>
                                <th scope="col" class="px-6 py-3">
                                    Name
                                </th>
                                <th scope="col" class="px-6 py-3">
                                    Email
                                </th>
                                <th scope="col" class="px-6 py-3">
                                    Specialty
                                </th>
                                <th scope="col" class="px-6 py-3">
                                    Action
                                </th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr class="bg-white border-b">
                                <th scope="row" class="px-6 py-4 font-medium">
                                    Doctor Name
                                </th>
                                <td class="px-6 py-4">
                                    doctor@gmail.com
                                </td>
                                <td class="px-6 py-4">
                                    Surgeon
                                </td>
                                <td class="px-6 py-4">
                                    Edit
                                </td>
                            </tr>

                        </tbody>
                    </table>
                </div>

                    </div>
                </div>
            </div>
    </AuthenticatedLayout>
</template>
